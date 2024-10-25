1. Autostart Teamcity server and agent after unexpected server shutdown. teamcity.service. 
Be careful with variables: user name and path. (my user is teamcity)

sudo nano /etc/systemd/system/teamcity.service

# sudo useradd -r -m teamcity (My user was created when installing TeamCity.)

sudo chown -R teamcity:teamcity /opt/TeamCity

sudo systemctl daemon-reload

sudo systemctl enable teamcity.service

sudo systemctl start teamcity.service

2.