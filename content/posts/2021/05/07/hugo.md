---
title: "我为什么要写博客，以及搭建过程"
date: 2021-05-07T06:30:46+08:00
tags: ["Hugo","折腾","博客"]
categories: ["博客修建"]
---

## 开始

现在在博客园已经写了大概一百多个博客文章了，也是写了很久的文章。但是一直觉得博客不是自己的，只是在一个平台上面写文章。所以一直想要自己搭建一个博客，但是同时又觉得维护起来非常麻烦。比如会考虑到什么域名，或者服务器费用的问题。所以一直没有开始搭建自己的个人博客。

之前就有了解过`hexo`这样的程序，能够很方便的搭建一个平台。但是服务器还是要自己购买维护的，虽然我有服务器，但是考虑到还有域名的麻烦，就完全不想折腾了。后来了解到了`hugo`，也就是目前用到的这个博客生成系统。

似乎还是不错的样子，但是也有一些问题，比如说图片的问题，在使用`Typora`写文章的时候，插入的图片并不会自动放到合适的位置。导致如果写文章的时候能够正常看到图片，那么使用`hugo`生成静态网页的时候图片又显示不出来了。这个问题大概智能使用图床解决，当然，还可以写个`Python`脚本来完成两者之间的转换。但是，还是比较麻烦的不是？

对于这个问题，我又想到了之前的`七牛云`的储存空间，最近一直有打电话问我是否会考虑他家的服务器或者储存空间。

上控制台发现如果要使用的话，还是需要一个域名。而我的域名才过期，，，真的是非常巧啊。明明有域名的时候用不到，但是需要域名的时候又没有。没办法，智能问学长借用一个二级域名了。这才配置好了图床。

然后写文章测试。本地测试没有问题，等我`push`到`github page`上面的时候，却打不开图片。`F12`可以看到说是`Mixed content`这样的问题。经过百度之后发现是因为在`https`网站使用`http`链接导致的。这就意味着我必须使用给学长的二级域名弄个证书。好在善良的学长二话不说给我弄好了。

但是上控制台发现，`https`流量要收费 并不是免费的。。。 可恶啊，都是套路.... 不过认真看了一下套餐发现，`1GB`的流量才收费`0.28元`和免费也没有什么区别了啊.... 看这七牛云`眉慈目善`的还真是靠谱。

于是，现在我就能使用`七牛云`和`github page`搭建自己的博客了。

---

实际上这篇文章是测试好平台之后的第一篇文章。也正好是做测试了，之后会逐渐把博客园的文章搬运过来。另外，之后写文章会好好写的，不能再写流水帐了。