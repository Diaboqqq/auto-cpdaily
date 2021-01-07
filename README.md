# 今日校园自动签到-云函数版

### 1、使用

下载：[下载链接1](https://share.neoniou.com/serverless.zip)

备用下载链接：[备用链接](http://neowmoe.huangenet.cn/download/serverless.zip)

请查看使用手册：https://blog.neoniou.com/posts/auto-serverless-readme/



### 2、更新记录

**2021.01.07**

感谢[链接](https://github.com/ZimoLoveShuang/auto-sign/issues/38)提供的DES key =w=，更新了新的des key

**2020.12.29**

增加了server酱的推送，可以将打卡结果推送到微信，下载最新版，然后[使用链接](https://blog.neoniou.com/posts/auto-serverless-readme/#6%E3%80%81%E9%85%8D%E7%BD%AE-Server%E9%85%B1%E6%8E%A8%E9%80%81)

**2020.12.25**

删除了很蠢的更新机制，更新了API，以后如果打卡失败请及时提醒我更新API。

关于腾讯云函数登录失败的问题，我猜测可能是定时任务的问题，可以的话把定时任务执行的cron表达式改为：

```
0 0 9,20 * * * *
```

这表示每天9点、20点执行一次，应该能够解决，目前也还在测试当中...

**2020.12.1**

新版

**2020.10.30**

更新了今日校园新的API

更新了从服务器获取最新API的逻辑，后续如果今日校园API再有变动，不用重新下载安装程序，只需等待服务端热更新API

**2020.10.23**

更新了今日校园新的API

**2020.7.23**

更新同一设备登录无法签到的问题