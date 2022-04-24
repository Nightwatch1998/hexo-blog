---
title: npm常用命令
date: 2022-04-22 16:43:00
tags:
categories: 常用命令行
---
## npm常用命令
+ npm install 安装模块
+ npm install 安装模块
+ npm uninstall卸载模块
+ npm root 查看包的安装路径
+ npm ls 查看安装的模块
+ npm view package version
+ npm init -y在项目中引导创建一个package.json文件
+ npm help 查看某条命令的详细帮助
+ npm root 查看包的安装路径
+ npm config 管理npm的配置路径
	+ 全局安装路径
		npm config set prefix "E:\Program Files x86\Nodejs\node_global"
	+ 全局缓存路径
		npm config set cache "E:\Program Files x86\Nodejs\node_cache"
+ npm version 查看模块版本
+ npm link 本地项目连接本地模块
	+ npm link
		在自定义包根目录下运行,会在npm全局安装目录下创建一份包的拷贝
	+ npm link packageName
		在需要使用的项目目录下
+ npm源
	npm get registry查看镜像源
	npm config set registry http://www.npmjs.org切换官方源
	npm config set registry http://registry.npm.taobao.org切换淘宝源
	npm install --registry=https://registry.npm.taobao.org使用临时淘宝源
+ nvm
	node版本管理工具
