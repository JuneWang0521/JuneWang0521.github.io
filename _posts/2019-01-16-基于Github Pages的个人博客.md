---
title: 基于Github Pages的个人博客
categories: 博客搭建
tags: 博客搭建
permalink: /JuneWang/_posts
---
## 引言

因为不想使用CSDN的博客，打算自己搭建一个博客，碰巧发现了不需要服务器的Github Pages，于是打算搭建一个个人博客。

参考了Negen大佬的[三步搭建自己的博客网站（GitHubPages + Jekyll）](https://www.jianshu.com/p/4048bbb259e9)(感谢大佬)。

## 一、创建 github 仓库

创建一个 github 仓库命名为你的账户名。例如，我的账户名是 JuneWang0521 ，那么就创建一个名为 JuneWang0521.github.io 的仓库，而且起名一定要按照这个格式。

![创建仓库](/public/image/2019-01-16-1.jpg)

创建完成后复制下面的地址，将仓库 clone 到本地。

```bash
git clone
```

![复制地址](/public/image/2019-01-16-2.jpg)

## 二、选择 jekyll 主题

到 [jekyll主题官网](http://jekyllthemes.org) 选择一个自己喜欢的主题，下载到本地。

页面如下：

![jekyll主题官网](/public/image/2019-01-16-3.jpg)

我选择了 [wu-kan](http://jekyllthemes.org/themes/wu-kan/) 作为我的博客页面主题。

点击 [download](https://github.com/wu-kan/wu-kan.github.io/archive/master.zip) 直接下载到本地。

![wu-kan主题](/public/image/2019-01-16-4.jpg)

将下载下来的主题解压到 github 仓库下面，解压后的仓库文件结构如下：

![文件结构](/public/image/2019-01-16-5.jpg)

##三、修改配置文件

修改配置文件`_config.yml`

个人认为比较主要的配置修改如下：

![修改配置](/public/image/2019-01-16-6.jpg)

##四、上传到 github 仓库

将修改后的主题 push 到 github

在仓库根目录下打开gitBash，执行以下语句

```bash
git add .
```
```bash
git commit -m "[init]初始化博客"
```
```bash
git push
```

上传成功后到 github 仓库点击 Settings。

![点击仓库](/public/image/2019-01-16-7.jpg)

等待页面自动刷新，出现一个url即是你的博客地址。

![博客地址](/public/image/2019-01-16-8.jpg)

##五、测试

点击博客地址即可进入到博客主页，效果如下:

![博客测试](/public/image/2019-01-16-9.jpg)

[测试地址](https://junewang0521.github.io/JuneWang0521.github.io/)

##六、发布第一篇博客

发布的博客都在文件夹`_post`下面：

![博客文件夹](/public/image/2019-01-16-10.jpg)

md文件命名格式：`年-月-日-标题.md`

文件里面的内容就是正常的markdown文件格式。

编辑完成就可以将更新的内容 push 到 github 上面了。

刷新博客主页，查看上传是否成功。
