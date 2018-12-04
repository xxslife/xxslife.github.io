---
title: OneDrive for Business 部署 OneIndex
date: 2018-11-11 15:01:57
categories: [OneDrive,OneIndex]
---

#### 1.注册一个 OneDrive for Business 账号，账号需要管理员，因为需要创建 API 权限。

#### 2.获取 OneDrive API

#####  登陆 [Azure Active Directory](https://manage.windowsazure.com/) 管理，注册新应用程序   ![oneindex_1](https://xxs.now.sh/?/Blog/OneIndex/oneindex_1.png)

<!-- more -->

##### 输入名称，OneDrive， 应用程序类型选择 Web 应用/API，登陆URL输入：[https://login.microsoftonline.com/](https://login.microsoftonline.com/)，然后创建

![oneindex_2](https://xxs.now.sh/?/Blog/OneIndex/oneindex_2.png)

##### 记录应用程序 ID 备用：

![oneindex_3](https://xxs.now.sh/?/Blog/OneIndex/oneindex_3.png)

##### 点击应用左上角设置，将右侧的回复 URL 修改为: [https://onedrive.live.com/about/business/](https://onedrive.live.com/about/business/)

![oneindex_5](https://xxs.now.sh/?/Blog/OneIndex/oneindex_5.png)

##### 点击所需权限 - Windows Azure Active Directory ，确认是否已选中 Sign in and user profile，如果没有则选中并点击完成：

![oneindex_6](https://xxs.now.sh/?/Blog/OneIndex/oneindex_6.png)

![oneindex_7](https://xxs.now.sh/?/Blog/OneIndex/oneindex_7.png)

##### 然后添加权限，API 选择 Office 365 SharePoint Online，启用访问权限勾选 Read user files 和 Read and write user files，点击完成授权：

![oneindex_8](https://xxs.now.sh/?/Blog/OneIndex/oneindex_8.png)

![oneindex_9](https://xxs.now.sh/?/Blog/OneIndex/oneindex_9.png)

![oneindex_10](https://xxs.now.sh/?/Blog/OneIndex/oneindex_10.png)

##### 点击密钥，填入密钥描述，如：OneDrive，持续时间选择年限 1 年（超过可能会出现异常），保存，然后记录密钥值备用：

![oneindex_11](https://xxs.now.sh/?/Blog/OneIndex/oneindex_11.png)

![oneindex_12](https://xxs.now.sh/?/Blog/OneIndex/oneindex_12.png)

##### 到这里 OneDrive for Business 上部署 OneIndex 就已经成功，下一步就是搭建 OneIndex 了。