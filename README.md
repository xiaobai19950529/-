# -

一，安装Nodejs

  1. Github上获取源码
  
     sudo git clone https://github.com/nodejs/node.git
     
     现在此方法不行
     cd node 
     sudo make uninstall
     
     可以直接去nodejs官网下载最新版本的nodejs
     然后在~/.bashrc里添加PATH
     
     sudo nano ~/.bashrc
     
     export PATH=$PATH:/home/xiaobai/Downloads/node-v6.11.0-linux-x64/bin

     source ~/.bashrc
     
     node -v 有版本号代表安装成功
     
     注意： bashrc 一劳永逸
          bash_profile 只在当前终端有效
     
     
  2. 修改目录权限
  
     sudo chmod -R 755 node
     
  3. 使用./configure创建编译文件
  
     sudo ./configure
     sudo make
     sudo make install
     
  4. 查看版本号
  
     node --version

二.安装mongodb

  https://docs.mongodb.com/manual/tutorial/install-mongodb-on-ubuntu/ 

三，安装Redis

  https://www.digitalocean.com/community/tutorials/how-to-install-and-configure-redis-on-ubuntu-16-04
  
  检测Redis是否安装成功（查看版本号）:
  
  服务端： redis-server -v
  客户端： redis-cli -v
  
四.安装JDK

  http://topspeedsnail.com/ubuntu16-install-java-jdk/
  
五.安装bower
  
  需先安装nodejs和npm
  
   sudo apt-get install nodejs npm git
   
   nodejs --version 
   npm --version
   
   sudo npm install -g bower
   
   bower --version
   
六.安装chrome浏览器

   在终端中，输入以下命令：

        wget -q -O - https://dl.google.com/linux/linux_signing_key.pub  | sudo apt-key add -

    导入谷歌软件的公钥，用于下面步骤中对下载软件进行验证。

    如果顺利的话，命令将返回“OK”

    sudo apt-get update

    用于对当前系统的可用更新列表进行更新。

    在终端中，输入以下命令：

            sudo apt-get install google-chrome-stable

    执行对谷歌 Chrome 浏览器（稳定版）的安装。


    在终端中执行以下命令：

    google-chrome-stable

    将会启动谷歌 Chrome 浏览器，它的图标将会出现在屏幕左侧,右键图标锁定到启动器即可。

