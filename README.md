# vue开发环境搭建Mac版
1、安装brew 
打开终端运行以下命令：
/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
安装成功后，查看一下brew的版本信息：
brew -v
注：我安装成功后，在查看brew的信息是出现”-bash: brew: command not found”,处理方法：解决mac安装homebrew后报错-bash: brew: command not found，还要说明一点的是，我没有vim去修改那个文件，我是直接找到那个文件用文本编辑器直接修改的。

2、安装node.js 
在终端中运行以下命令：

brew install nodejs
也可以下载后安装： 
下载地址：https://nodejs.org/en/download/

安装成功后，查看一下node.js的版本信息：

node -v

3、获取nodejs模块安装目录访问权限

　sudo chmod -R 777 /usr/local/lib/node_modules/
 
4、安装 淘宝镜像 （npm）

npm install -g cnpm --registry=https://registry.npm.taobao.org

5、安装webpack

cnpm install webpack -g

6、安装vue脚手架

npm install vue-cli -g

7、在硬盘上找一个文件夹放工程用的，在终端中进入该目录

cd 目录路径

8、根据模板创建项目

vue init webpack-simple 工程名字<工程名字不能用中文>
如下
vue init webpack-simple demo1

会有一些初始化的设置，如下输入: 
Target directory exists. Continue? (Y/n)直接回车默认(然后会下载 vue2.0模板，这里可能需要连代理) 
Project name (vue-test)直接回车默认 
Project description (A Vue.js project) 直接回车默认 
Author 写你自己的名字

cd 命令进入创建的工程目录

cd demo1

注意：最后三步都是要进入到当前工程目录后执行的。

9、安装项目依赖

npm install

比较慢，需要有点耐心……

10、安装 vue 路由模块vue-router和网络请求模块vue-resource

cnpm install vue-router vue-resource --save

11、启动项目

npm run dev
