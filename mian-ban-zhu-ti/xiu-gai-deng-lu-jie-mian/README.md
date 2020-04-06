# 登陆界面修改

第一步：去[模板之家](http://www.cssmoban.com/tags.asp?n=%E7%99%BB%E5%BD%95)挑一个你喜欢的登陆模板并下载。

![](https://imgs.lovpass.cn/img/2020/01/28/e5060a298342520200128.jpg)

第二步：找到`index.html`文件，右键选择用记事本或者用npp打开。并在`</body>`的末尾前加上以下内容：

```text
<script type="text/javascript" src="../common/jquery-3.2.1.min.js"></script>
<script type="text/javascript" src="../common/URL.js"></script>
<script type="text/javascript" src="../common/md5.js"></script>
<script type="text/javascript" src="../common/js/login.js"></script>
```

![](https://imgs.lovpass.cn/img/2020/01/28/6a11a9a2b94c520200128.jpg)

第三步：在用户名的`<input>`标签里面加上`id="login-userid"`。  
 密码的`<input>`标签里面加上`id="login-passwd"`。  
 最后在登录按钮里加上`id="login-button" onclick="MCSERVER.btnLogin()"`。

![](https://imgs.lovpass.cn/img/2020/01/28/98dd73e403c4320200128.jpg)

最后，把面板目录下默认的登陆文件夹`./public/login`里面的文件删掉，并把你刚才改好的登陆界面丢进去，完事~

