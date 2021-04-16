Linux系统网络重装。
脚本原作者大佬的网站一直在维护，在这里整理一下，方便自用。

# 以在Debian9下重装Debian9为例，以下为重装步骤：

## 首先确保安装了所需软件
```
apt update
apt install -y xz-utils openssl gawk file wget ca-certificates screen
```

## 开一个名为screen00的screen
```
screen -S screen00
```

## 然后下载脚本并给其权限
```
wget https://raw.githubusercontent.com/XfZGGG/installNET/master/InstallNET.sh && chmod a+x InstallNET.sh
```

## 运行脚本
```
bash InstallNET.sh -d 9 -v 64 -a
```
### 或者
```
bash InstallNET.sh -d 9 -v 64 -a -p 'Passwd4root' -- mirror 'http://ftp.jp.debian.org/debian/'
```
回车后耐心等待重装……
直到完成。
