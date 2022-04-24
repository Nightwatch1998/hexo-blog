---
title: hexo标签插件(tag-plugins)
date: 2022-04-24 11:22:01
categories: 
- 博客写作
tags:
- hexo
---

## 引用块
```
{% blockquote [author[, source]] [link] [source_link_title] %}
content
{% endblockquote %}
```

{% blockquote [author[, source]] [link] [source_link_title] %}
content
{% endblockquote %}

### 引用书上的句子
```
{% blockquote David Levithan, Wide Awake %}
Do not just seek happiness for yourself. Seek happiness for all. Through kindness. Through mercy.
{% endblockquote %}
```
{% blockquote David Levithan, Wide Awake %}
Do not just seek happiness for yourself. Seek happiness for all. Through kindness. Through mercy.
{% endblockquote %}

## 代码块
在文章中插入代码
```
{% codeblock [title] [lang:language] [url] [link text] [additional options] %}
code snippet
{% endcodeblock %}
```
### 普通的代码块
```
{% codeblock %}
alert('Hello World!');
{% endcodeblock %}
```
{% codeblock %}
alert('Hello World!');
{% endcodeblock %}
### 指定语言
```
{% codeblock lang:javascript %}
function component() {
    const element = document.createElement('div');
    const btn = document.createElement('button');

    // lodash 在当前Script中使用import 引入
    element.innerHTML = _.join(['Hello', 'webpack','字体','测试'], ' ');
    btn.innerHTML = 'Click me and check the console'
    btn.onclick = printMe;

    element.appendChild(btn);

    return element;
}
{% endcodeblock %}
```
{% codeblock lang:javascript %}
function component() {
    const element = document.createElement('div');
    const btn = document.createElement('button');

    // lodash 在当前Script中使用import 引入
    element.innerHTML = _.join(['Hello', 'webpack','字体','测试'], ' ');
    btn.innerHTML = 'Click me and check the console'
    btn.onclick = printMe;

    element.appendChild(btn);

    return element;
}
{% endcodeblock %}
### 附加说明和网址
```
{% codeblock _.compact http://underscorejs.org/#compact Underscore.js %}
_.compact([0, 1, false, 2, '', 3]);
=> [1, 2, 3]
{% endcodeblock %}
```
{% codeblock _.compact http://underscorejs.org/#compact Underscore.js %}
_.compact([0, 1, false, 2, '', 3]);
=> [1, 2, 3]
{% endcodeblock %}


