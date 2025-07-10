\# ELK Stack Security Lab



This project sets up a security-focused ELK (Elasticsearch, Logstash, Kibana) stack using Vagrant and VirtualBox, with two VMs:

\- \*\*Kali Linux\*\* for generating attack/test logs.

\- \*\*Ubuntu\*\* with Filebeat/Logstash/Elasticsearch/Kibana.



\## 🔧 Lab Architecture



\- Kali: `192.168.56.10`

\- Ubuntu (ELK): `192.168.56.11`

\- Log forwarding: Filebeat → Logstash → Elasticsearch → Kibana

\- Kibana UI: \[http://192.168.56.11:5601](http://192.168.56.11:5601)



\## 🧰 Tech Stack



\- Vagrant + VirtualBox

\- Kali Linux (`kalilinux/rolling`)

\- Ubuntu 18.04 (`ubuntu/bionic64`)

\- ELK Stack (7.x)

\- Filebeat for log shipping

\- Grok filters for Apache log parsing



\## 🚀 Getting Started



```bash

git clone https://github.com/YOUR-USERNAME/elk-stack-security-lab.git

cd elk-stack-security-lab

vagrant up

Then access Kibana at: http://192.168.56.11:5601

