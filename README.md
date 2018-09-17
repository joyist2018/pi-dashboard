# Pi Dashboard
A WebUI dashboard for IoT devices likes raspberry pi.

Project details: (http://maker.quwj.com/project/10)

Copyright 2017 NXEZ.com.

安装方法
安装共2步，首先安装 Nginx（或 Apache）和 PHP。然后在 Nginx 目录通过 SFTP 或 GitHub 部署好本项目的程序。
1.安装 Nginx 和 PHP
2.部署 Pi Dashboard
这里介绍两种方法将 Pi Dashboard 部署在 Nginx 上。
2.1. SFTP 上传
在 GitHub 下载本项目源码。通过 FileZilla 等 FTP 软件将解压出来的目录上传到web根目录下。
那么可以通过 http://IP地址/pi-dashboard 访问部署好了的 Pi Dashboard。
如果页面无法显示，可以尝试在树莓派终端给源码添加运行权限，例如你上传之后的路径是 /var/www/html/pi-dashboard，则运行。
cd /var/www/html
sudo chown -R www-data pi-dashboard

2.2. GitHub 部署
如果你了解过 GitHub 的基本操作，通过 GitHub 来下载本项目到 Pi 上会相当方便。

#如果已安装过 git 客户端可以跳过下一行
sudo apt-get install git
cd /var/www/html
sudo git clone https://github.com/spoonysonny/pi-dashboard.git

即可通过 http://IP地址/pi-dashboard 访问部署好了的 Pi Dashboard。

同样如果页面无法显示，可以尝试在树莓派终端给源码添加运行权限，例如你上传之后的路径是 /var/www/html/pi-dashboard，则运行。

cd /var/www/html
sudo chown -R www-data pi-dashboard

========================================
一下是自用克隆源代码，需要的请自助安装。

//克隆可道云
[root@centos-rpi2 10.0.0.8]# git clone https://github.com/kalcaddle/KODExplorer.git
Cloning into 'KODExplorer'...
remote: Counting objects: 11523, done.
remote: Compressing objects: 100% (544/544), done.
remote: Total 11523 (delta 253), reused 563 (delta 155), pack-reused 10759
Receiving objects: 100% (11523/11523), 49.03 MiB | 647.00 KiB/s, done.
Resolving deltas: 100% (6152/6152), done.
Checking out files: 100% (1256/1256), done.
[root@centos-rpi2 10.0.0.8]# chmod -Rf 777 ./KODExplorer/*

==================
//克隆DzzOffice开源办公套件
[root@centos-rpi2 10.0.0.8]# git clone https://github.com/zyx0814/dzzoffice.git
Cloning into 'dzzoffice'...
remote: Counting objects: 7502, done.
remote: Compressing objects: 100% (262/262), done.
remote: Total 7502 (delta 65), reused 149 (delta 48), pack-reused 7167
Receiving objects: 100% (7502/7502), 35.60 MiB | 1.74 MiB/s, done.
Resolving deltas: 100% (1965/1965), done.
Checking out files: 100% (3390/3390), done.
[root@centos-rpi2 10.0.0.8]# chmod -Rf 777 ./*

==================
//克隆XiunoBBS -轻论坛 
[root@centos-rpi2 10.0.0.8]# git clone https://gitee.com/xiuno/xiunobbs.git        
Cloning into 'xiunobbs'...
remote: Enumerating objects: 15371, done.
remote: Counting objects: 100% (15371/15371), done.
remote: Compressing objects: 100% (5914/5914), done.
remote: Total 15371 (delta 10362), reused 13269 (delta 9001)
Receiving objects: 100% (15371/15371), 35.86 MiB | 1.33 MiB/s, done.
Resolving deltas: 100% (10362/10362), done.
[root@centos-rpi2 10.0.0.8]# chmod -Rf 777 ./xiunobbs/*

==================
//克隆Typecho博客平台
[root@centos-rpi2 10.0.0.8]# git clone https://github.com/typecho/typecho.git
Cloning into 'typecho'...
remote: Counting objects: 8794, done.
remote: Compressing objects: 100% (6/6), done.
remote: Total 8794 (delta 0), reused 0 (delta 0), pack-reused 8788
Receiving objects: 100% (8794/8794), 7.79 MiB | 903.00 KiB/s, done.
Resolving deltas: 100% (6079/6079), done.
[root@centos-rpi2 10.0.0.8]# chmod -Rf 777 ./typecho/*
[root@centos-rpi2 10.0.0.8]# 

主题 ：
大前端 https://git.coding.net/Arco-X/DUX-for-Typecho.git
大姐姐 https://git.coding.net/Arco-X/H-Code.git
https://github.com/chakhsu/pinghsu.git

插件：
标签自动生成 https://github.com/DT27/AutoTags.git
Markdown 编辑器 https://github.com/DT27/EditorMD.git
==================
//爱特PHP网站文件管理专家
[root@centos-rpi2 10.0.0.8]# wget https://aite.me/fileadmin.zip
[root@centos-rpi2 10.0.0.8]# unzip fileadmin.zip
[root@centos-rpi2 10.0.0.8]# chmod -Rf 777 ./*

==================
//克隆FluxBB -轻论坛 
[root@centos-rpi2 10.0.0.8]# git clone https://github.com/fluxbb/fluxbb.git
[root@centos-rpi2 10.0.0.8]# chmod -Rf 777 ./*

语言包https://github.com/fluxbb/langs
==================
//克隆Pi Dashboard (Pi 仪表盘) IoT 设备监控工具，提供 Web UI 仪表盘面板
[root@centos-rpi2 10.0.0.8]# git clone https://github.com/joyist2018/pi-dashboard.git  （中文版源）
https://github.com/spoonysonny/pi-dashboard.git （英文版源）

[root@centos-rpi2 10.0.0.8]# chmod -Rf 777 ./*

==================
//克隆HTML5 Speedtest 网站测速
[root@centos-rpi2 10.0.0.8]# git clone https://github.com/adolfintel/speedtest.git
[root@centos-rpi2 10.0.0.8]# chmod -Rf 777 ./*

==================
//克隆 ImgURL轻便图床源码
[root@centos-rpi2 10.0.0.8]# git clone https://github.com/helloxz/imgurl.git
[root@centos-rpi2 10.0.0.8]# chmod -Rf 777 ./*




