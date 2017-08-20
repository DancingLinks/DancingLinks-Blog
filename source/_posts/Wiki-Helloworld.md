---
title: Wiki&Helloworld!
date: 2017-08-21 00:06:04
tags: 
  - about
  - qianyu
categories: about
---

## 我们终于有Wiki了

咸鱼了三年之后，终于搭建起了ACM-Wiki，这是咸鱼的一大步。

首先介绍一下使用方法：

1. 首先克隆本仓库：https://github.com/DancingLinks/ACM-Wiki.git

2. 需要npm，可以百度下环境搭建，可能需要npm install

3. 关于Hexo的环境搭建可以参考这里：http://www.jianshu.com/p/465830080ea9

之后就可以在本地编辑文件了

### Create a new post

``` bash
$ hexo new "My New Post"
```

More info: [Writing](https://hexo.io/docs/writing.html)

### Run server

``` bash
$ hexo server
```

More info: [Server](https://hexo.io/docs/server.html)

### Generate static files

``` bash
$ hexo generate
```

More info: [Generating](https://hexo.io/docs/generating.html)

### Deploy to remote sites

注意一下，这里需要npm install hexo-deployer-git --save

``` bash
$ hexo deploy
```

More info: [Deployment](https://hexo.io/docs/deployment.html)

### 总结

基本每次只要按这个流程来就好了

``` bash
$ hexo new "My New Post"
$ hexo clean
$ hexo generate
$ hexo deploy
```

### 风格

首先我们需要tag，初步设想的一个作者tag、一个分类tag，其他也可以补充，改日再议。

然后分知识-模板-题解-原题。思路是原题就不要贴了，直接用传送门就好了，然后模版和题解之间也可以用传送门- -
