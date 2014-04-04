---
layout: post
title: 使用jekyll和github搭建blog(亲试成功)
---
# 使用jekyll和github搭建blog
@(Study)[github, jekyll, blog]

OS|Version|
-|-|
Ubuntu|12.04-64bit

## 1. 安装jekyll
### 1.1 安装ruby


`$ sudo apt-get install ruby irb rdoc`


### 1.2 安装gem


`$sudo apt-get install rubygems-1.9.1`

### 1.3 使用gem安装Jekyll

`$sudo apt-get install ruby1.9.1-dev`

`$gem install jekyll`



## 2. 写blog

参考: http://skyinlayer.com/blog/2014/01/27/jekyll-2/
### 2.1 新建markdown博客
**新建blog/目录:**

`$jekyll new blog`

在`_posts`新建`_posts/2014-04-04-hello.markdown`.
内容:
```
---
layout: post                                                                                                                                     
title: 第一篇
---

使用jekyll+github搭建博客成功，以后要写点东西了.
```
### 2.2 使用jekyll编译blog

```
$cd blog
$jekyll build
```
生成`_site`目录， 博客就放在`_site`目录下。

### 2.3 本地预览blog
运行jekyll server， 然后访问`http://0.0.0.0:4000`, 即可预览到blog效果。
```
$jekyll serve
```

## 3. 将blog放到github

### 3.1 在github新建repository
命名必须为`username.github.io`如: `azhe12.github.io`

### 3.2 将本地blog放到github

注意`branch`必须为`mater`.

```
$cd blog

$git init

$git add .

$git commit -m "first blog"

$git push

$git remote add origin git@github.com:azhe12/azhe12.github.io.git

$git push origin master
```


