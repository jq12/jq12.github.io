---
title: Commonly used software install Manual
tags:
- ubuntu
- install
---
<!--more-->

## uget

````

sudo add-apt-repository ppa:plushuang-tw/uget-stable

sudo add-apt-repository ppa:t-tujikawa/ppa

#uGet client install

sudo apt-get install uget

#depend aria2

sudo apt-get install aria2
````
## Cili BT Xtunder client isntall (Ktorent)
````
sudo apt-get install ktorrent

sudo apt-get install amule

#transfer Xtunder  code to ori url
echo #QUFlZDJrOi8vfGZpbGV8JUU4JUExJThDJUU1JUIwJUI4JUU4JUI1JUIwJUU4JTgyJTg5LlRoZS5XYWxraW5nLkRlYWQuUzA2RTAxLiVFNCVCOCVBRCVFOCU4QiVCMSVFNSVBRCU5NyVFNSVCOSU5NS5IRFRWcmlwLjEwMjR4NTc2Lm1wNHw2NDg3NTg1MDl8ZjIyZmI2OTRjMDQ0ZmYyNjU0MjhhNTEzNWVhYzhiOTB8aD12eXFsNHFjNHpmYmx0eWNqdW1rcnNibDJza2JscTJsZnwvWlo= #| base64 -d

##add anaconda3 env
export PATH=/home/develop/anaconda3/bin:$PATH
````


## mount the second disk
````
mount /dev/vdb /u01

#这时候如果磁盘之前挂载过，是挂载不上的，报下面的错
我们要初始化磁盘

mkfs.ext4 /dev/vdb

````
##add anaconda env to  jupyter notebook

````
#list all conda env
 conda env list
#activate env which you are desired to used in jupyter
activeate  evn.name
#instal ipykernel
conda env Injection
python -m ipykernel install --user --name your_env --display-name "Python [conda env:your_env]"
your_env 是你的conda环境名称
Python [conda env:your_env]：将是你在notebook中看到的名称。
````
##Sublime Text 3

1. Open terminal via Ctrl+Alt+T or by searching for “Terminal” from desktop app launcher. When it opens, run command to install the key:
```
wget -qO - https://download.sublimetext.com/sublimehq-pub.gpg | sudo apt-key add -

sublimetext-apt-key
```
2. Then add the apt repository via command:
```
echo "deb https://download.sublimetext.com/ apt/stable/" | sudo tee /etc/apt/sources.list.d/sublime-text.list

sublime text apt repository
```
3. Finally check updates and install sublime-text via your system package manager:
```
sudo apt-get update

sudo apt-get install sublime-text
```
Uninstall:

`sudo apt-get remove sublime-text && sudo apt-get autoremove`

## or run:
````
 sudo apt-key adv --keyserver keyserver.ubuntu.com --recv-keys BA300B7755AFCFAE

wget -qO - https://typora.io/linux/public-key.asc | sudo apt-key add -

# add Typora's repository

sudo add-apt-repository 'deb https://typora.io/linux ./'

sudo apt-get update

# install typora

sudo apt-get install typora
````
