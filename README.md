# CUBE CDR
Cisco CDR analyse with ELK-stack. 

Based on [Justin Jahn's configuration file](https://gist.github.com/justinjahn/85305bc7b7df9a6412baedce5f1a0ece)

Add next configuration to Cisco border element.
```
gw-accounting syslog
logging host 192.168.1.1 transport udp port 10514
```
Install [translate plugin](https://www.elastic.co/guide/en/logstash/current/plugins-filters-translate.html).
Rsyslog is used to store logs for a long period of time and logstash for real-time analyzing for a last week.
Add configuration of rsyslog, logrotate and logstash. 
Import Kibana visualization.

# SCREENSHOTS

![Visualize](visualize.png?raw=true "Visualize")

