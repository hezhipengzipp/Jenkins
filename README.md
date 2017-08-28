# Jenkins+gradle+svn+windows自动化编译、上传svn#
Jenkins+android+gradle+svn构建项目自动化打包、编译及上传到svn.由于公司开发需求，研发人员给测试人员发出svn源码路径、svn版本号，测试人员构建自动化打包、
编译apk文件自动上传到svn上。
Jenkins每次打包的build号、打包源码svn路径、版本号需要自动注入到apk文件。方便线上出现了bug,可以及时追溯源码路径。
if  you have any issue,send email to zippsun@126.com,thanks.
# 开发背景 #
	最近公司业务需求比较少，空闲下来。把之前搭建jenkins分享给大家，虽然网上也有很多关于这方面的资料。但是这篇文章有网上没有的
	**apk注入svn源码路径、版本号、jenkins build号**
## 需求介绍 ##
	1.由于公司开发需求，研发人员给测试人员发出svn源码路径、svn版本号，测试人员构建自动化打包、
	编译apk文件自动上传到svn上。
	2.为了追溯线上问题，apk文件需要注入编译svn源码路径、版本号以及jenkins build号。
## 搭建 ##
	*Jenkins下载地址：https://jenkins.io/download/，里面有两个安装版本：LTS(稳定版本)和Weekly(开发版本)，Weekly版本每周
	*都会更新的，我们选择LTS的，避免以后使用中出现问题。

![点击下载](https://raw.githubusercontent.com/hezhipengzipp/Jenkins/master/download.png)<br>
	*点击windows版或者.war，windows启动时通过dos命令行方式启动的，而war包是可以通过tomcat服务器启动的
