---
title: Listen 1 音乐播放器
date: 2019-01-11 20:27:27
tags: 音乐
categories: App
---



![](https://xxs.now.sh/?/Blog/TopPicture/top_2.png)

<!-- more -->

## 写在前面

随着音乐版权意识提高，现在想听歌需要去不同音乐平台，如果你是使用客户端的话，通常需要下载两到三家平台的 App。今天推荐的 Listen 1 是一个可以让你使用一个播放器同时搜索并试听包括 网易云音乐，虾米音乐，QQ音乐等六个主流平台的歌曲的 App。更重要的是 Listen 1 可以全平台使用，包括 Chrome 插件，Firefox 插件，Windows 32位和64位版本，Mac 版本以及 Linux 32位和64位版本。

## 伸手就来

点击 [Listen 1](http://listen1.github.io/listen1/) 进入官网下载

## 自己动手

因为 Listen 1 是开源的，所以你也可以自己动手打包，这里就简单介绍一下 macOS 版本的打包流程。

### 第一步：checkout 代码

前往 https://github.com/listen1 checkout [listen1_desktop](https://github.com/listen1/listen1_desktop) 的代码到本地。

> 这里需要特别注意一个问题，README 里说到 “因为项目中包含了 listen1_chrome_extension 的引用，在checkout后需要把引用库初始化 git submodule update --init --recursive” 。执行这段代码有时候莫名其妙的比较慢，并且后面打包也有莫名其妙的问题，所以建议直接去 checkout  [listen1_chrome_extension](https://github.com/listen1/listen1_chrome_extension) 然后把里面的文件拷贝到 “listen1_desktop/app/listen1_chrome_extension“ 目录下

### 第二步：安装 electron-builder
终端进入  listen1_desktop 目录，执行 `yarn add electron-builder --dev` 命令

### 第三步：生成 macOS 安装包
等待 electron-builder 安装完成后，终端中执行 `npm run dist:mac` 命令，就会看到 listen1_desktop 目录下多了一个 dist 的文件夹，等待终端运行完，即可在文件夹中看到生成的安装包 `Listen1_2.1.2_mac.dmg`

