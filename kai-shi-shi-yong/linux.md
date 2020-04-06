# Linux

## 运行在Ubuntu

### 第零步

#### 输入`sudo -i`切换到`root`用户

![](https://imgs.lovpass.cn/img/2019/08/04/5d46d3fc5b340.jpg)

### 第一步

#### 输入`apt update`更新包

![](https://imgs.lovpass.cn/img/2019/08/04/5d46d3fd2f5c9.jpg)

### 第二步

#### 输入`apt install nodejs`安装`nodejs`

#### 装完后记得输入`node -v`检查版本，如果没显示那就重装一次。如果版本过低[请看这里](https://blog.imlazy.ink:233/index.php/archives/58/)

![](https://imgs.lovpass.cn/img/2019/08/04/5d46d3fd26e35.jpg)

### 第三步

#### 输入`apt install git`安装`git` 

![](https://imgs.lovpass.cn/img/2019/08/04/5d46d3fdaf74e.jpg)

### 第四步 \[可选\]

#### 输入`apt install npm`安装`npm`  ![](https://imgs.lovpass.cn/img/2019/08/04/5d46d3fd664d1.jpg)

### 第五步

#### 输入：`git clone https://github.com/Suwings/MCSManager.git`克隆源码

![](https://imgs.lovpass.cn/img/2019/08/04/5d46d3fe18d1b.jpg)

### 第六步

#### 输入`cd MCSManager`进入程序根目录，然后执行命令`npm install`，如果提示`-bash: npm: command not found`就去执行第四步

![](https://imgs.lovpass.cn/img/2019/08/04/5d46d3fc468fd.jpg)

### 第七步

#### 执行命令`node app.js`或者`npm start`启动面板

![](https://imgs.lovpass.cn/img/2019/08/04/5d46d3fca3acd.jpg)

### 最后一步

打开浏览器输入[127.0.0.1:23333](http://127.0.0.1:23333/)  
然后输入默认账号：`#master`密码：`123456`就可以进入面板啦！

如果你还是不会，可以考虑我的[付费安装]()服务![](https://tb2.bdstatic.com/tb/editor/images/face/i_f25.png?t=20140803)

## 运行在Centos / RedHat <a id="centos"></a>

### 第一步

用`root`用户连接到你的CentOS服务器 \[如果是本机就用`sudo -i`切换到`root`用户\]。

![image](https://i.zerodream.net/66f4f3ee45784e4a62ff6d728ebdd8f5.jpg)

### 第二步

输入`yum -y install git`安装`git`工具。

![image](https://i.zerodream.net/fe11dac671aed0d0bfe0166345439162.jpg)

### 第三步

输入`yum -y groupinstall "Development Tools"`安装`Development Tools`。

![image](https://i.zerodream.net/36cddce4c50f526809dbd0f5755b26a6.jpg)

### 第四步 \[可选\] 

输入`yum -y install wget`安装`wget`工具。

![image](https://i.zerodream.net/8438aa1dd6eee45ca98c9d8ccf4f532f.jpg)

### 第五步：

输入`wget https://npm.taobao.org/mirrors/node/v11.0.0/node-v11.0.0.tar.gz`从淘宝镜像下载`Nodejs`。  
如果出现`-bash: wget: command not found`的情况请重复第四步\]。

![image](https://i.zerodream.net/9c0f0704bb39471c848999cdc60ddbd8.jpg)

### 第六步：

#### 输入命令`tar -xvf node-v11.0.0.tar.gz`解压安装包。

![image](https://i.zerodream.net/68ef3c9018500c6d059cfc2fe62d10db.jpg)

### 第七步

输入命令`cd node-v11.0.0`进入目录。

![image](https://i.zerodream.net/991acc5f9d77987eaac85b55408c8d0b.jpg)

### 第八步：

输入命令`yum install gcc gcc-c++`安装Gcc-c++插件。

![image](https://i.zerodream.net/d5d41c8e83019763f0ededbb2fadd46a.jpg)

### 第九步：

输入命令`./configure`使用默认配置。

![image](https://i.zerodream.net/7b7ebf052bed9a345480e44bb92678a8.jpg)

### 第十步：

输入`make`进行编译。\[可能需要差不多半小时\]

![image](https://i.zerodream.net/0c0c6fc3d71c713c05e830dec8520b2b.jpg)

### 第十一步：

输入命令`make install`开始安装Nodejs

![image](https://i.zerodream.net/5bca64fcafa4f58df3798d6cd0f356df.jpg)

### 第十二步：

输入`node -v`检查Nodejs是否安装成功  
如果显示`-bash: node: command not found`请重复第十步，出现版本号即为安装成功

![image](https://i.zerodream.net/d463185f2ec104f46ea5ec165f605f5f.jpg)

### 第十三步：

`git clone https://github.com/Suwings/MCSManager.git`克隆源码

![image](https://i.zerodream.net/617cd624e3caef8b9d13e4eb491fc364.jpg)

### 第十四步：

输入命令`cd MCSManager`进入程序根目录，然后执行命令`npm install --production`

![image](https://i.zerodream.net/36a451ac6ce65035ba517ff4ce6239f9.jpg)

### 第十五步

输入`npm start`或者`node app.js`就能启动面板了

![image](https://i.zerodream.net/7b1adcb1e44a3bb445b225a2c4c87dfd.jpg)

### 第十六步：

#### 打开浏览器访问 http://你的服务器地址:23333 就能进入面板了。如果是本机测试就访问[127.0.0.1:23333](http://127.0.0.1:23333/)然后输入默认账号：`#master`密码：`123456`就可以进入面板啦！

无法访问？请[点击这里](error/canthttp.html)

## 在后台保持运行

先安装`screen`软件

Ubuntu：`sudo apt install screen`  
CentOS：`yum install screen`

然后创建一个名字叫做mcsm的窗口

最后`npm start`启动你的面板

如果与终端断开连接，可以使用`screen -r mcsm`重新连接

