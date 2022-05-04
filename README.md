# linux
linux bspwm polybar


将你的mpd用户名添加到你的登录组和音频组：

$ sudo gpasswd -a mpd

$ chmod 710 ~/

$ sudo gpasswd -a mpd audio

通过启动mpd测试配置文件是否有效：

$ mpd

$ ss -tunelp | grep 6600

tcp    LISTEN     0 5 127.0.0.1:6600  *:* users:(("mpd",pid=10906,fd=8)) uid:1000 ino:269403 sk:8

mpd.service systemd单元可用于/usr/lib/systemd/system/mpd.service上的autostart。

