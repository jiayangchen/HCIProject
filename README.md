# HCI Project

### Introduction

Architecture diagram

![image](http://o9oomuync.bkt.clouddn.com/hcihciinf.png)

This is an app designed to recognize your emotion and then recommend corresponding emoijs to you, which can help you quickly pick emoij images. It uses the <a href="https://azure.microsoft.com/zh-cn/services/cognitive-services/">Project Oxford API</a> and <a href="http://www.emokit.com/">EmoKit</a> Tool to recognize a user's emotion. In order to speed up the processing, I use Redis to cache some emotion data ahead of time. And try to use the data given by local Emokit Tool to compare with the data cached in Redis. If they have a high degree of similarity between them, then we needn't get data through internet request, which will save a lot of time. The app can also share emoij images between two users by scanning QRCode generated by each other.

### ChatKit

ChatKit 是由 LeanCloud 官方推出的、基于 [LeanCloud 实时通信 SDK「LeanMessage」](https://leancloud.cn/docs/leanstorage_guide-android.html) 开发并封装了简单 UI  的聊天套件。它可以帮助开发者快速掌握 LeanMessage 的技术细节，轻松扩展和实现常用的聊天功能。

ChatKit 是一个免费且开源的项目组件，提供完全自由的授权协议，开发者可以对其进行任意的自定义和二次封装。ChatKit 的底层依然基于 LeanCloud 为各平台推出的 SDK，其最大特点是把聊天常用的一些功能配合 UI 一起提供给开发者。

使用方法请参考[官方文档](https://leancloud.cn/docs/chatkit-android.html)。


