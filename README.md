# elk-pfsense
A small collection of Logstash configurations to support pFsense 2.4.3 and dashboard visualizations within Kibana.

![alt text](https://github.com/8270647/elk-pfsense/blob/master/kibana-dashboard-visu.JPG)

# Versions

- Ubuntu Server 18.04
- pFsense 2.4.3
- Elastic 6.3.0
- Logstash 6.3.0-1
- Kibiana 6.3.0

# Installation

- <b>Assumption</b>: fully functioning ELK 6+ install on Ubuntu 18.04. Many guides already exist (e.g. http://pfelk.3ilson.com/)
- Copy the contents of the /conf.d folder to your local logstash installation path (e.g. /etc/logstash/conf.d)
- Cope the contents of the /patterns folder to your local logstash installation path (e.g. /etc/logstash/patterns)

# Patters

While many versions of the Grok patters to support pfsense 2.4.+ exist, the following is confirmed working as of July 01, 2018. The supplied patters file (pfsense2-4.grok) assumes you are using vlans within your pfsense environment (it should work without vlans as well)
