1. Autostart Teamcity server and agent after unexpected server shutdown. teamcity.service. 

sudo nano /etc/systemd/system/teamcity.service

sudo chown -R teamcity:teamcity /opt/TeamCity

sudo systemctl daemon-reload

sudo systemctl enable teamcity.service

sudo systemctl start teamcity.service
