---
title: 天命之子 PC 端代理方法
date: 2020-03-02 17:22:54
tags: DestinyChild
categories: Games
---

> ★注意：如果使用 岛风Go/ACGP，这两个软件会自动帮你修改 .\rt\lib\net.properties 文件，所以请先将 DMM安装目录下 .\rt\lib\net.properties 替换成未被修改的版本 [「点我下载 提起码：zero」](https://pan.baidu.com/s/1fyflQOE1mxQbxudqiomUhw) 

## 0x00 软件环境

- ##### 系统 Windows 10

- ##### Proxifier [「点我下载 提起码：zero」](https://pan.baidu.com/s/13c_2WGTBmkKSNmnNRfASyA)

- ##### 任意科学上网工具


## 0x01 配置过程
#### 1. 首先打开代理服务器配置
![代理服务器](1.png)
#### 2. IP 填 127.0.0.1，端口看自己科学上网的本地端口
![ip和端口](2.png)
#### 3. 代理服务器配置完成图
![代理服务器配置完成图](3.png)
#### 4. 接下来配置代理规则
![代理规则](4.png)
#### 5. 将 dmm 进程加入代理规则中，①处填写 dmm 的进程（dmmgameplayer.exe） ②处选择服务器，也就是刚才添加的
![dmmgameplayer.exe](5.png)
#### 6. 将 dc 进程加入代理规则中，①处填写 dc 的进程（Destiny.exe） ②处选择服务器，也就是刚才添加的
![Destiny.exe](6.png)
#### 7. Default 选择 Direct
![Default](7.png)
#### 8. 代理规则配置完成图
![代理规则配置完成图](8.png)
#### 9. 这时候启动 dmm 就可以游戏了 

## 0x02 写在最后
每次游戏前 需要先打开 科学上网软件 和 Proxifier
