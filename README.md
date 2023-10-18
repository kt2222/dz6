# dz6
<b>rsyslog->logstash->kibana</b><br>
Install elasticsearch;<br>
Install kibana;<br>
Add elastic certs to kibana directory;<br>
Install logstash;<br>
Add input.conf, output.conf to /etc/logstash/conf.d/;<br>
Add 01-json-template.conf, ssh.conf to /etc/rsyslog.d/<br>
sudo systemctl restart rsyslog.service
sudo systemctl restart logstash
Open kibana https://elk.fat123.keenetic.pro
Management -> Index Management -> ssh_logs_for_elastic-2023.10 -> <br>
-> ManageIndex -> Add lifecycle policy -> logs -> <br>
-> Analytics -> Discover -> ssh_logs_for_elastic-2023.10 -> <br>
-> Visualize Library -> Create visualization -> Lens = Done
