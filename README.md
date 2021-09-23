# Ubuntu 20.04 note !

Sử dụng lệnh usermod để thêm user vào group sudo :
  usermod -aG sudo itadmin
Sử dụng lệnh adduser để thêm user mới vào hệ thống của bạn:
  adduser itadmin 

# Ubuntu Linux firewall
  sudo ufw status verbose
To allow incoming tcp packets on port 22
  sudo ufw allow 22/tcp
To open http and https service
  sudo ufw allow http
  sudo ufw allow https
To open port
  sudo ufw allow 53
  sudo ufw allow from 192.168.1.10 to any port 22
Available applications:
  Nginx Full
  Nginx HTTP
  Nginx HTTPS
  Squid
Denying/blocking port access
  sudo ufw deny 25
  sudo ufw deny 25/tcp comment 'Block access to smptd by default
Delete ufw rules
  sudo ufw status
  sudo ufw numbered
  sudo ufw delete {num}
  sudo ufw delete allow 80
sudo ufw default allow outgoing
sudo ufw default deny incoming
sudo ufw allow ssh
sudo ufw enable
sudo ufw disable


