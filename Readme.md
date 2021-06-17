![Shadowsocks](https://github.com/teddysun/shadowsocks_install/raw/master/shadowsocks.png)
# Auto install Shadowsocks Server

shadowsocks.sh
===============
- Auto Install Shadowsocks(Python) Server for CentOS/Debian/Ubuntu
- https://teddysun.com/342.html

shadowsocks-libev.sh
===============
- Auto Install Shadowsocks(libev) Server for CentOS
- https://teddysun.com/357.html

shadowsocks-libev-debian.sh
===============
- Auto Install Shadowsocks(libev) Server for Debian/Ubuntu
- https://teddysun.com/358.html

shadowsocks-go.sh
===============
- Auto Install Shadowsocks(Go) Server for CentOS/Debian/Ubuntu
- https://teddysun.com/392.html

shadowsocks-crond.sh
===============
- Check Shadowsocks(All version) Server is running or not, and start it if not running
- https://teddysun.com/525.html

shadowsocksR.sh
===============
- Auto Install ShadowsocksR Server for CentOS/Debian/Ubuntu
- https://shadowsocks.be/9.html
```
安装wget --no-check-certificate https://raw.githubusercontent.com/teddysun/shadowsocks_install/master/shadowsocksR.sh
chmod +x shadowsocksR.sh
./shadowsocksR.sh 2>&1 | tee shadowsocksR.log
卸载./shadowsocksR.sh uninstall
启动：/etc/init.d/shadowsocks start
停止：/etc/init.d/shadowsocks stop
重启：/etc/init.d/shadowsocks restart
状态：/etc/init.d/shadowsocks status

配置文件路径：/etc/shadowsocks.json
日志文件路径：/var/log/shadowsocks.log
代码安装目录：/usr/local/shadowsocks
```
多用户配置示例：

{
"server":"0.0.0.0",
"server_ipv6": "[::]",
"local_address":"127.0.0.1",
"local_port":1080,
"port_password":{
    "8989":"password1",
    "8990":"password2",
    "8991":"password3"
},
"timeout":300,
"method":"aes-256-cfb",
"protocol": "origin",
"protocol_param": "",
"obfs": "plain",
"obfs_param": "",
"redirect": "",
"dns_ipv6": false,
"fast_open": false,
"workers": 1
}
```
如果你想修改配置文件，请参考：
https://github.com/shadowsocksr-backup/shadowsocks-rss/wiki/Server-Setup
https://github.com/shadowsocksr-backup/shadowsocks-rss/blob/master/ssr.md
https://github.com/shadowsocksr-backup/shadowsocks-rss/wiki/config.json


shadowsocks-all.sh
==================
- Auto Install Shadowsocks Server (all version) for CentOS/Debian/Ubuntu
- https://teddysun.com/486.html

haproxy.sh
===============
- Auto Install haproxy for Shadowsocks Server
- https://shadowsocks.be/10.html

Copyright (C) 2014-2019 Teddysun
