# 网易云音乐linux版下载及ubuntu下安装

[网易云音乐下载](http://music.163.com/#/download)  
点击上方链接进行下载

下载对应deb包，使用快捷键ctrl+alt+t打开终端，打开下载目录  
执行以下命令:

`sudo dpkg -i netease-cloud-music_0.9.0-1_amd64.deb` 

如果出现以下错误：

```shell
dpkg: 依赖关系问题使得 netease-cloud-music 的配置工作不能继续：
netease-cloud-music 依赖于 libcue1；然而：
未安装软件包 libcue1。
netease-cloud-music 依赖于 libqt5x11extras5 (>= 5.1.0)；然而：
未安装软件包 libqt5x11extras5。
dpkg: 处理软件包 netease-cloud-music (--install)时出错：
依赖关系问题 - 仍未被配置
正在处理用于 mime-support (3.54ubuntu1.1) 的触发器 ...
正在处理用于 gnome-menus (3.10.1-0ubuntu2) 的触发器 ...
正在处理用于 desktop-file-utils (0.22-1ubuntu1) 的触发器 ...
正在处理用于 bamfdaemon (0.5.1+14.04.20140409-0ubuntu1) 的触发器 ...
Rebuilding /usr/share/applications/bamf-2.index...
正在处理用于 hicolor-icon-theme (0.13-1) 的触发器 ...
在处理时有错误发生：
netease-cloud-music
```

那么执行如下命令：

`sudo apt-get -f install`

下面是个人安装成功的屏幕截图：  
![netease-cloud-music](http://o7s72jtji.bkt.clouddn.com/netease.png)
