# 石墨文档“文件夹分享”插件

## 2017-03-17 更新

因为这个插件没人在用，所以决定关闭服务器，并将服务端代码开源。

服务端代码：https://github.com/ionepub/shimo-fav-server

如果有需要的，可以自己搭建一个服务端。

**自己搭建的服务端，只需要修改`/js/background.js`中的`baseUrl`变量值为自己的服务端地址即可。**

```javascript
var baseUrl = "http://shimofav.applinzi.com/";
```

---------------

这是一个chrome浏览器扩展程序，使用它可以便捷地分享石墨文档(https://shimo.im)的文件夹中所有非私有的文档。

效果：

![](https://dn-shimo-image.qbox.me/QsPuYwbBvM0aqojx/share.gif)

![](https://dn-shimo-image.qbox.me/pUuu8vHFLJ4W4QzA/shared.gif)

![](https://dn-shimo-image.qbox.me/wwXAMO5Ys58lfQIm/cancel.gif)

## 说明

- 服务器搭建在新浪sae上，在程序上做了一些安全性处理，但是**不保证数据绝对安全**
- 插件仅上传被分享文件夹内的**非私有**文档、表格和文件夹的**标题**（非私有意即文档是只读或者可写的，私有文档数据不会被共享）
- 插件不会对文档、表格的内容做任何操作，包括读取其内容
- 分享之后的文件夹即使用户不登录石墨文档也可以查看
- 对文件夹有 **重命名、新增、删除、权限调整** 操作时，需要“更新分享”
- 对文档、表格内容的所有修改，不需要“更新分享”

> 如果自己对插件源码做了调整，从而导致隐私数据泄露等问题概不负责。

## 使用方法

**直接将已分享的文件夹URL地址发送给同样安装有插件的人即可。**

### Google chrome

目前没有发布到谷歌浏览器插件平台，使用以下方式安装。

- 下载shimo-fav.crx文件
- 打开谷歌浏览器，在地址栏中输入 ` chrome://extensions  ` 进入插件页面，或从右上角菜单进入更多工具-扩展程序
- 将shimo-fav.crx文件拖动到浏览器中，提示安装
- 安装完成之后即可使用

### QQ浏览器

- 下载shimo-fav.crx文件
- 打开QQ浏览器，在地址栏中输入 ` qqbrowser://extensions/manage  ` 进入插件页面，或从右上角菜单进入应用中心-管理我的应用
- 将shimo-fav.crx文件拖动到浏览器中，提示安装
- 安装完成之后即可使用

### 其他浏览器

凡带有chrome内核的浏览器一般都支持此插件，如果直接安装crx文件失败，可下载源码后使用浏览器开发者模式加载插件

------------------------
