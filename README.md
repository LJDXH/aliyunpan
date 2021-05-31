# 阿里云盘小白羊版

20210531冒个泡，我在认真编码哦：

最新版下载：[v1.5.31 https://wwe.lanzoui.com/b01npsg8h](https://wwe.lanzoui.com/b01npsg8h)

旧版下载：[v1.5.25 https://wwe.lanzoui.com/b01nqc4gd](https://wwe.lanzoui.com/b01nqc4gd)

<br />
:o:定个小目标：下次满 `150` Star就更新:o:
<br />
<br />

``````
0531 已完成功能：
1.支持 扫码登录/Cookie登录
2.支持 阿里云盘基本功能(列出文件/重命名/移动/回收站/收藏夹)
3.支持 在线预览全格式原画视频（非转码）,在线预览图片
4.支持 批量下载文件/文件夹，多文件同时下载+断点续传。满速下载
5.支持 上传文件/文件夹，多文件并发上传+断点续传

开发中功能：
秒传链接分享功能
``````

<br />

![ui](https://files.xiami.com/musician-avatar/07d8ec1a38a5462c3afbfac41413b8af/a7a5f9bd75333768990a48931fd4f6d3-846x558.gif)

<br />

截图看不了的话自己点：[截图视频](https://files.xiami.com/musician-avatar/07d8ec1a38a5462c3afbfac41413b8af/a7a5f9bd75333768990a48931fd4f6d3-846x558.gif)
 
 <br />
  
``````
功能规划：
5. 秒传链接创建和保存，分享
6. 文件自动加密功能、洗码功能
7. 离线下载功能
``````

<br />

``````
秒传链接：
1.可以一键创建单个文件、多个文件、单个文件夹、多个文件夹、文件+文件夹混排的秒传链接
2.可以创建秒传链接的短链接（一个文件要有sha1#文件大小#文件名，很多文件会导致链接超级长），短连接只有20位字符
3.可以设置秒传短链接的有效期（N天有效，N次保存有效），密码（有自定义密码、无密码），可以附加备注信息
4.可以粘贴短链接保存文件到自己的网盘内、可以粘贴标准秒传链接保存文件到自己的网盘内
``````

<br />

``````
对上传文件预处理，自动加密、洗码功能
1.可以对文件洗码，上传前选择洗码，会自动在文件末尾附加随机长度0字节，导致文件sha1码，文件长度都随机，也就是生成唯一的新的sha1码（视频文件洗码后不影响在线预览功能）
2.可以对文件加密，上传前选择加密，会自动对文件进行异或加密，导致文件sha1码更新且文件无法预览（视频文件无法预览，无法生成截图，图片/文本/doc/pdf等等文件无法在线预览）
3.对加密后的文件，在下载时会自动解密，也会提供单独的解密程序。保证以后随时可以自己独立解密，并且因为是随机密码异或加密，速度超级快！！
``````

<br />

``````
离线下载：
1.可以自己一键配置离线服务器、使用公共离线服务器。实现电驴、磁力链接的下载
2.可以下载后自动上传到自己的网盘内
``````
<br />

#### 项目说明

这是一个基于阿里云盘的客户端项目，功能参照6盘小白羊第二版，

1. 增加秒传链接功能（创建秒传链接--分享给别人，和使用秒传链接--保存到自己的阿里云盘里）。

2. 增加离线下载功能（仅支持 磁力、电驴）提交磁力链接，离线保存到自己的阿里云盘里。

此项目由我个人开发，为的是学习flutter2框架


#### 功能规划

1. 开发 客户端，复刻小白羊功能（基于阿里云盘）
2. 开发 Aria服务端，提交磁力链接，使用aria2下载后自动上传到阿里云盘，并生成秒传链接

最后，会将服务端打包好，方便大家用最简单的步骤自行搭建服务端（也会开放我自己搭建的服务端供大家免费调用）




