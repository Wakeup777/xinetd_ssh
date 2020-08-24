just put the config in  /etc/xinetd.d/, turn off ssh and turn on xinetd via systemctl. Check who is managing ssh via lsof -i :22
