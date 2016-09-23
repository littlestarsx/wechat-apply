# wechat-apply
wechat-apply  微信小程序初体验（IDE的安装以及安装过程的常见问题）

###本文主要参照[github/gavinkwoe](https://github.com/gavinkwoe/weapp-ide-crack)

###所需文件

IDE 0.7和0.9版本 + crack-master.zip + demo.zip

###文件下载地址

#####开发工具 v0.7

百度: https://pan.baidu.com/s/1pLxqFzH （密码: bwt9）

360: https://yunpan.cn/ckvTYFHWzYYFV （提取码：e09b）

#####开发工具 v0.9

百度: https://pan.baidu.com/s/1pLTKIqJ （密码: iswg）

360: https://yunpan.cn/ckvXjEbnFYMSC （提取码：f9ca）


1. 安装IDE 0.7 和IDE 0.9

2. 替换0.9版本的文件（weapp-ide-crack-master.zip）

```
    Windows：

        \package.nw\app\dist\components\create\createstep.js

        \package.nw\app\dist\stroes\projectStores.js

        \package.nw\app\dist\weapp\appservice\asdebug.js

    Mac：

        /Resources/app.nw/app/dist/components/create/createstep.js

        /Resources/app.nw/app/dist/stroes/projectStores.js

        /Resources/app.nw/app/dist/weapp/appservice/asdebug.js
```

3. 扫码登录
无法登录问题 please bind your wechat account to the appid first
使用0.7扫码登录，在登录0.9即可解决

4. 创建项目
AppID：随便填
项目名称：随便填
本地开发目录：选择一个目录
点击「添加项目」
此时如果出错，先退出再重进
此时，能够看到项目列表了

5. 打开刚刚创建项目文件所在目录，覆盖demo(WechatAppDemo)

6. 关闭开发工具，重新打开

####错误解决方案

修复asdebug.js报错
问题原因：TypeError: Cannot read property 'MaxRequestConcurrent' of undefined

win解决方案：替换 \package.nw\app\dist\weapp\appservice\asdebug.js

mac解决方案：替换 /Resources/app.nw/app/dist/weapp/appservice/asdebug.js