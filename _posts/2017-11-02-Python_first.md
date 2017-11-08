---
layout: post
title: python
date: 2017-11-02 
tags: 编程
---


### 变量与字符串

　　变量的名字叫做标识符。大小写敏感     

```     
file = open('D:/GitHub/file.txt','w')
file.write('hello world!')
```         

|python 对文件的单词统计

```
import string  # 引入string模块
path = 'C:\users\Edoit\Desktop\Walden.txt'  # 设置文件路径变量

with open(path, 'r') as text:    # 以'r'打开路径
    
    words = [raw_word.strip(string.punctuation).lower() for raw_word in text.read().split()]  # 使用列表推导式/解析式 循环遍历文档的内容以空格split and strip 标点符号 and lower的格式生成list
    words_index = set(words)     # set集合函数自动去除重复元素
    count_dict = {index: words.count(index) for index in words_index} # 创建一个以单词为key，出现次数为value的字典
for word in sorted(count_dict, key=lambda x: count_dict[x], reverse=True): # 打印
    print('{} -- {} times'.format(word, count_dict[word]))

```　　

### 一些基本语法


标题            
H1 :# Header 1            
H2 :## Header 2           
H3 :### Header 3           
H4 :#### Header 4           
H5 :##### Header 5            
H6 :###### Header 6      
链接 :[Title](URL)        
加粗 :**Bold**        
斜体字 :*Italics*         
*删除线 :~~text~~          
段落 : 段落之间空一行           
换行符 : 一行结束时输入两个空格           
列表 :* 添加星号成为一个新的列表项。          
引用 :> 引用内容               
内嵌代码 : `alert('Hello World');`        
画水平线 (HR) :--------          
           

css 的大部分语法同样可以在 markdown 上使用，但不同的渲染器渲染出来的 markdown 内容样式也不一样，下面这些链接里面有 markdown 基本语法，你也可以在下面几个平台上尝试着写一些。

### 一些好用的 Markdown 编辑器

<br />

[MaHua](http://mahua.jser.me/?utm_source=mindstore.io) 在线 Markdown 编辑器 ,无须测试。


<br />

![](/images/posts/markdown/image1.png)

<br />

[Markdown Plus](http://mdp.tylingsoft.com/) 一款 Markdown 编辑器，可以支持添加任务列表、emoji、流程图等。

<br />

![](/images/posts/markdown/image2.png)

<br />

[Cmd Markdown](https://www.zybuluo.com/cmd/?utm_source=mindstore.io) 作业部落在线 Markdown 编辑器推出桌面版客户端啦，全平台支援。

![](/images/posts/markdown/image3.png)

[Macdown](https://github.com/MacDownApp/macdown) Github 上开源的 Mac 平台上的 Markdown 编辑器

[GitBook Editor](https://www.gitbook.com/editor?utm_source=mindstore.io) 一款团队在线编辑文档工具。可以轻松书写笔记，支持团队协同编辑。同时支持 Markdown 语法，还保持了印象笔记的风格并可在线预览。


[Outlinely](http://www.glamdevelopment.com/outlinely?utm_source=mindstore.io) 界面简洁大方的大纲类 Mac 软件，使用起来很简单，而且支持输出 Markdown 格式。


[Classeur](http://classeur.io/?utm_source=mindstore.io) 实用简洁的 Markdown 写作工具，快速上手。


[DeerResume](https://github.com/geekcompany/DeerResume?utm_source=mindstore.io) 程序员专用 MarkDown 简历制作在线工具。                

<br>