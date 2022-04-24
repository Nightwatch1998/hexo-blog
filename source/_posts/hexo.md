---
title: hexo个人博客部署
date: 2022-04-22 16:43:00
tags:
categories: 常用命令行
---

---
## 安装hexo
+ npm i -g hexo-cli
    并将hexo-cli加入环境变量
+ npm i -S hexo-deployer-git
    安装git部署插件
### 目录结构
1. _config.yml
    网站配置信息
2. scaffolds
    模板文件夹
3. source
    + 资源文件夹
    + categories 分类
    + tags 标签
    + about 关于
    + resources 资源
4. themes
    主题文件夹

---
## 部署相关
1. 部署到GitHub
	deploy  repository: https://github.com/Nightwatch1998/Blog.git
2. 解析域名
	阿里云控制台域名，添加解析记录
3. 未绑定域名是生成的网址不区分大小写
---

## 更换主题
+ 使用next主题
    repository: https://github.com/Nightwatch1998/Nightwatch1998.github.io.git
    然后在themes/next的_config.yml中配置schemes
---
## 命令
+ hexo init
    在空的文件夹下初始化
+ hexo clean
    清除缓存文件和已生成的静态文件public
+ hexo publish
    发表草稿
+ hexo new page "pagename"
    再sources下创建新的文件夹
+ hexo generate/hexo g
    生成静态文件到public文件夹
+ hexo server/hexo s
    本地启动服务器
+ hexo deploy/hexo d
    部署网站，会自动把本地public文件夹提交到github仓库
---
## 配置themes/next
1. 菜单
    menu
    || 前面是路由，后面是图标名称，来自
2. 建站时间
    since
3. 设置头像
    avatar
    本地文件或URL
4. 网站图标
    favicon
5. 动态背景设置
    + canvas nest
        git clone https://github.com/theme-next/theme-next-canvas-nest source/lib/canvas-nest
    + 3D library
        git clone https://github.com/theme-next/theme-next-three source/lib/three
6. 设置背景图片
    style
        style: source/_data/styles.styl
    会寻找  souce/css目录
7. 主页文章添加阴影效果
8. 添加顶部加载条
    git clone https://github.com/theme-next/theme-next-pace source/lib/pace
    pace
9. 侧边栏显示效果
    sidebar
10. 侧边栏推荐阅读
    links
11. 社交链接
    social
12. 设置博文内链接为蓝色
    themes/next/source/css/_common/components/post/post.styl
13. 显示文章字数和阅读时长
    npm install hexo-wordcount --save
14. 添加评论功能
    https://www.livere.com/my_Livere
    暂时不用
