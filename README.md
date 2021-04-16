Linux系统网络重装。
脚本原作者大佬的网站一直在维护，在这里整理一下，方便自用。
***
~~(以Debian为例)
向导式重装：
```
wget https://raw.githubusercontent.com/XfZGGG/installNET/master/Install.sh
chmod +x Install.sh
./Install.sh
```
按提示操作。
等待…… 直到完成。~~

***
(以在Debian下重装Debian为例)
非向导式重装：
首先确保安装了脚本所需软件
```
apt update
apt install -y xz-utils openssl gawk file
```
然后下载脚本并给其权限
```
wget https://raw.githubusercontent.com/XfZGGG/installNET/master/InstallNET.sh && chmod a+x InstallNET.sh
```

可选步骤，开一个名为screen01的screen，并准备在其中运行脚本
```
apt install screen -y
screen -S screen01
```

运行，重装
```
bash InstallNET.sh -d 9 -v 64 -a -p 'root密码' -- mirror 'http://ftp.jp.debian.org/debian/'
```

等待……
直到完成。
