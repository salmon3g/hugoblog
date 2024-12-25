---
title: 给博客增加了Twikoo评论系统
description: 最近抽时间增加了评论系统，对比和调研了多个评论系统，最后选择了 Twikoo。美中不足略有遗憾的是，之前的所有评论都没有了，只能重新来过。
categories: [life]
tags: ["hugo"]
draft: false
slug: ""
date: "2024-07-07 20:31:14"
---

两年前，把博客从 Typecho 迁移到了 Hugo，[Bye Typecho, Hello hugo](https://wangdongxing.com/life/bye-typecho-hello-hugo/)，和 Typecho、WordPress 不同的是，Hugo 不带评论系统。博客不能失去评论系统，就像西方不能失去耶路撒冷。

最近不太忙，抽时间增加了评论系统，对比和调研了多个评论系统，最后选择了 Twikoo。美中不足略有遗憾的是，之前的所有评论都没有了，只能重新来过。

Twikoo评论系统使用起来也很方便，具体可见官方的文档：[Twikoo文档](https://twikoo.js.org/quick-start.html)，基本流程如下：

1. 申请 MongoDB 账号，并创建数据库
2. 申请 Vercel 账号
3. 将 Twikoo 一键部署到 Vercel
4. 在 Vercel 中的一些配置
5. 将 Twikoo 代码添加到 single.html 中

大功告成，欢迎留个脚印再走~

2024-09-03 update

可能是因为部署在 Vercel 的原因，现在评论加载有些慢，后面有时间再优化。
