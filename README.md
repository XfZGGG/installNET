这是一个简陋的Linux系统网络重装脚本。
原作者大佬的网站一直在维护，整理了一下，主要是方便自己用。
***
(以Debian为例)
向导式重装：
```
wget https://raw.githubusercontent.com/XfZGGG/installNET/master/Install.sh
chmod +x Install.sh
./Install.sh
```
按提示操作。
等待…… 直到完成。
***
(以在Debian下重装Debian为例)
非向导式重装：
首先确保安装了脚本所需软件
```
apt update
apt install -y xz-utils openssl gawk file
```
然后下载脚本
```
wget https://raw.githubusercontent.com/XfZGGG/installNET/master/InstallNET.sh
```

可选步骤，开一个名为screen01的screen，并准备在其中运行脚本
```
apt install screen -y
screen -S screen01
```

运行，重装
```
bash InstallNET.sh -d 10 -v 64 -a -p '[这里填密码]'
```

等待……
直到完成。
