# mdsserver

## what's this ?
Mobile Data System (Blackberry service) Server can fix your 9000,8700...connect to network!

## how to use
``` c
git clone https://github.com/YangShuqing/mdsserver.git
cd mdsserver
gcc -Wall -o mds_server mds_server.c
sudo cp mds_server /usr/local/bin/
/usr/local/bin/mds_server
```

```c 
sudo touch /var/log/mds_server.log
sudo chown nobody /var/log/mds_server.log
sudo sed -i '/^exit 0/isu nobody -c "nohup /usr/local/bin/mds_server >>/var/log/mds_server.log &"' /etc/rc.local
```

##copyright
this is a fork from https://code.google.com/archive/p/ptcoding/

you can also refer to http://blog.ptsang.net/blackberry_broken_net_fix_server_for_linux


