just put the config in  /etc/xinetd.d/, turn off ssh and turn on xinetd via systemctl. Check who is managing ssh via lsof -i :22


systemctl stop sshd.service
systemctl start xinetd
lsof -i :22

for persistent setting use systemctl disable/enable


PS 

for systemd-service systemctl stop sshd.socket
