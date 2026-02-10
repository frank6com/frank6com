+++
date = '2026-02-09T23:54:38+08:00'
draft = true
title = 'Romm IGDB API 错误一例'
+++


### 前言

最近在使用 Romm 部署模拟器 Docker，按照官方文档部署后遇到了 IGDB API 错误，无法正常获取游戏信息。经过排查，发现是因为 IGDB API 的接口提供服务器非科学上网无法访问的问题，下面说一下解决过程。

### IGDB API 配置方法

Romm 的 IGDB API 配置其实很简单，大致逻辑就是通过 Twitch 账号登录 IGDB 并进入 Twitch 开发者平台创建一个应用，获取 Client ID 和 Client Secret 后填入 Romm Docker 的配置信息中即可。

#### 1. 登录 Twitch 开发者平台

首先需要一个 Twitch 账号，登录后进入 [Twitch 开发者平台](https://dev.twitch.tv/console/apps)，点击“Register Your Application”注册一个新的应用。

#### 2. 创建应用

在创建应用的过程中，需要填写一些基本信息：