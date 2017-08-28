#Jenkins+gradle+svn+windows自动化编译、上传svn
	最近公司业务需求比较少，空闲下来。把之前搭建jenkins分享给大家，虽然网上也有很多关于这方面的资料。但是这篇文章有网上没有的
	**apk注入svn源码路径、版本号、jenkins build号**
## 需求介绍 ##
	1.由于公司开发需求，研发人员给测试人员发出svn源码路径、svn版本号，测试人员构建自动化打包、
	编译apk文件自动上传到svn上。
	2.为了追溯线上问题，apk文件需要注入编译svn源码路径、版本号以及jenkins build号。
## 搭建 ##
	Jenkins下载地址：https://jenkins.io/download/，里面有两个安装版本：LTS(稳定版本)和Weekly(开发版本)，Weekly版本每周
	都会更新的，我们选择LTS的，避免以后使用中出现问题。

![点击下载](file:download.png)
