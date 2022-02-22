# Ansible
We use ansible as our configuration as code solution this challenge is to write a playbook to initialize a Amazon Linux 2 Server with the following:
- Install Filebeat
- Install MySQL
- Install Datadog Agent

There will be two servers that will need provisioning
mysql01.patronchallenge.io and 
mysql02.patronchallenge.io

# Filebeat Role
- This should send journal logs to a logstash server logstash.patronchallenge.io
- This should send mysql logs to that same server
- This should send cloud-init logs to that same server

# MYSQL Role
This should install MYSQL on the machine with the default configuration mysql01 should have "MYSQL8.0" installed while mysql02 should have "MySQL5.7"

# Datadog Agent
This should install the datadog agent on the instances and add the mysql check in the list of custom checks.