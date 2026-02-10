+++
date = '2026-02-10T14:55:10+08:00'
draft = false
title = 'Realink 真实链接转换'
tags = ['tempermonkey', '油猴脚本']
comments = true
+++

### 前言

常常在一些网站上看到连接名称是 `https://www.example.com`，但点击后却跳转到 `https://www.example.com/redirect?url=https%3A%2F%2Fwww.real-link.com` 之类的广告链接，所以我写了这样的一个脚本自动将这些链接替换成原本的真实链接。

### 实现逻辑

实现了一个简单的逻辑，就是在页面加载完成后，遍历所有链接，如果链接的 `href` 属性和要显示的链接文本不一致，就将 `href` 替换成链接文本。

### 发布

我已经发布到 Greasy Fork 上了，欢迎使用和反馈：
[Realink 真实链接转换](https://greasyfork.org/zh-CN/scripts/456789-realink-%E7%9C%9F%E5%AE%9E%E9%93%BE%E6%8E%A5%E8%BD%AC%E6%8D%A2%E8%84%9A%E6%9C%AC)。

### 未来计划

目前这个脚本的功能比较简单，未来可能会根据反馈使用情况增加一些功能，比如：

- 支持特定网站的链接替换规则
- 提供一个界面让用户自定义链接替换规则
- 优化性能，避免对大量链接进行不必要的替换

### 贡献

如果你有兴趣参与这个项目，欢迎在 GitHub 上提交 issue 或 pull request：
[GitHub 仓库地址](https://github.com/frank6com/realink).