---
title: Markdown的用法
date: 2021-7-19 18:00:00
categories: 
- web前端
tags: markdown
---
记性不好，用这种方式来加强印象


## 标题
1.使用=和-标记一级标题和二级标题
```
===============
---------------
```
2.使用#标记1-6级标题
```
#
##
###
####
#####
######
```

## 段落格式

### 段落
段落的换行是使用两个以上空格加上回车，或者直接空一行
### 字体
可以使用以下几种字体
```
*斜体文本*
_斜体文本_
**粗体文本**
——粗体文本——
***粗斜体文本***
___粗斜体文本___
```
*斜体文本*
_斜体文本_
**粗体文本**
——粗体文本——
***粗斜体文本***
___粗斜体文本___

### 分隔线
在一行中用三个及以上的星号、减号、底线来建立一个分隔线，可以加入空格
```
***
* * * 
******
- - - 
------------
```
### 删除线
在文字两端加上两个波浪线
```
~~删除线~~
```
~~删除线~~
### 下划线
通过HTML的\<u\>标签来实现
```
<u>带下划线的文本</u>
```
<u>带下划线的文本</u>
### 脚注
脚注的格式是
```
[^要注明的文本]
```
## 列表
1.Markdown支持有序列表和无序列表
无序列表使用星号、加号或者减号作为标记，标记后添加一个空格
```
* 第一项
* 第二项
* 第三项

+ 第一项
+ 第二项
+ 第三项


- 第一项
- 第二项
- 第三项
```
* 第一项
* 第二项
* 第三项

+ 第一项
+ 第二项
+ 第三项


- 第一项
- 第二项
- 第三项
2.有序列表使用数字加上.号来表示：
```
1. 第一项
2. 第二项
3. 第三项
```
1. 第一项
2. 第二项
3. 第三项
3.列表嵌套
列表嵌套只需在子列表选项前添加四个空格即可
```
1. 第一项：
    - 第一个元素
    - 第二个元素
2. 第二项：
    - 第一个元素
    - 第二个元素
```

## 区块
Markdown区块引用是在段落开头使用>符号,然后加一个空格
```
>区块
>用起来
>像这样
```
>区块
>用起来
>像这样
区块也可以进行嵌套，列表和区块可以相互嵌套

## 代码
一行使用反引号\`，多行使用三个反引号\`\`\`

## 链接
链接使用方法如下：
```
[链接名称](链接地址)
<链接地址>
```
## 图片
Markdown图片语法格式如下：
```
![alt 属性文本](图片地址)
![alt 属性文本](图片地址 "可选标题")
```
例如：
![alt 属性文本](http://img.doutula.com/production/uploads/image/2020/07/20/20200720214725_RbpMAz.jpg "可选标题")
调节宽高时需要使用\<img\>标签
## 表格
表格的使用有点特殊，语法格式如下，特别像评论区写生：
```
| 表头 | 表头 |
| ---  | ---  |
| 单元格 | 单元格 |
| 单元格 | 单元格 |
```
就像这样

| 表头 | 表头 |
| ----  | ----  |
| 单元格 | 单元格 |
| 单元格 | 单元格 |






