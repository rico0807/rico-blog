+++
author = "Rico0807"
title = "基于Netlify构建博客"
date = "2023-05-25"
description = "本篇博客主要介绍如何在Netlify上部署博客网站"
tags = [
	"Netlify",
]
series = ["Themes Guide"]
aliases = ["migrate-from-jekyl"]
image = "pawel-czerwinski-8uZPynIu-rQ-unsplash.jpg"

+++

## 基于Netlify构建博客

> 雨果官网：https://themes.gohugo.io/
>
> Netlify官网：https://app.netlify.com/
>
> Git官网：https://git-scm.com/

基本步骤：

> Step_01：在雨果官网中找到合适的Hugo网站模板，打开后点击Download，在进入的Github链接中选择fork到自己的Github库中
>
> Step_02：在Netlify网站中 Add Sites，网站源选择Github，导入成功后即可打开网站
>
> Step_03：根据个人需求，更新或改写模板网站中的内容

## 基于Git更新GitHub库

基本步骤：

> Step_01：在根目录下打开 Git Bash
>
> Step_02：将GitHub库中的工程文件下载至根目录
>
> Step_03：在下载好的文件中对源码进行修改
>
> Step_04：上传

```gas
git clone [url]

git add *
git commit -m "change"
git push [url] master
```

【注】：

> 1.在执行`git commit -m "change"`报错时，一般是 user.name 和 user.email未定义，通常使用`git config --global user.name xxxx`和`git config --global user.email xxxx`进行定义。
>
> 2.在第一次执行`git push [url] master`后会出现GitHub的授权或登录界面，按要求授权或登录即可完成更新上传。
>
> 3.上传是出现丢失服务等报错时，产生原因：一般是因为服务器的SSL证书没有经过第三方机构的签署，可使用`git config --global http.sslVerify "false"`，解除SSL验证后，再次git即可。
