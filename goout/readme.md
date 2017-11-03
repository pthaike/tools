# shadowsocks

https://github.com/shadowsocks/shadowsocks

windows 链接：http://pan.baidu.com/s/1bpo7XwV 密码：komp

apk 链接：http://pan.baidu.com/s/1kU5ClM3 密码：ixo9


## install in Ubuntu
```
apt-get install python-pip
pip install git+https://github.com/shadowsocks/shadowsocks.git@master
```


Create a config file /etc/shadowsocks.json. Example:
```
{
    "server":"my_server_ip",
    "server_port":8388,
    "local_address": "127.0.0.1",
    "local_port":1080,
    "password":"mypassword",
    "timeout":300,
    "method":"aes-256-cfb",
    "fast_open": false
}
```


To run in the background:
```
ssserver -c /etc/shadowsocks.json -d start
ssserver -c /etc/shadowsocks.json -d stop
```