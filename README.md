# 快捷命令 V0.0.1

## 简介

自定义可以在`uTools`中快速执行的命令或脚本

## 功能

#### 快速启动

可以配置一些常用的命令，比如`回收站` `查看网络连接`之类

![UTOOLS1556779074409.png](https://i.loli.net/2019/05/02/5cca904684757.png)

![UTOOLS1556779310377.png](https://i.loli.net/2019/05/02/5cca91329a525.png)

![UTOOLS1556779348048.png](https://i.loli.net/2019/05/02/5cca9155a2244.png)

![UTOOLS1556779660316.png](https://i.loli.net/2019/05/02/5cca928f51905.png)

配合`uTools`的全局功能快捷键，可以达到一键启动的功能

#### 常用脚本

如果为了一个小功能，就去编写一个插件，成本太高，本插件可以利用本地的脚本环境快速实现一些小功能。比如`base64转图片`等

![UTOOLS1556779835126.png](https://i.loli.net/2019/05/02/5cca933de1883.png)

目前可以添加以下类型的脚本，但要注意的是**本插件未封装任何运行环境，需要本机安装了环境才能执行相应的脚本**

![UTOOLS1556779901749.png](https://i.loli.net/2019/05/02/5cca938100c91.png)

同时，本插件可以作为一个便捷的脚本仓库，因为所有的脚本都是多设备自动同步的，无须另外存储在硬盘中

#### 输出处理

如果脚本有输出，则可以对输出内容做如下处理

- 忽略输出
- 显示纯文本输出 (不解析 html 内容)
- 显示html格式的输出 (可以进一步编写简单的 GUI 界面)
- 复制到剪贴板
- 发送到活动窗口

#### 插值变量

如果你仔细看了上面例子中的脚本，一定会发现很多脚本里都有`{{}}`格式的变量

本插件内置了一些特殊的插值变量，可以获取一些特殊的值，能够加入到插件里的任意脚本中

- `{{isWin}}` 是否是window系统
- `{{pwd}}` 资源管理器或访达的当前目录
- `{{ChromeUrl}}` 谷歌浏览器的当前链接
- `{{ClipText}}` 获取剪贴板的文本
- `{{SelectText}}` 获取选中的文本
- `{{SelectFile}}` 获取选中的文件 (单文件)
- `{{input}} ` 获取uTools主输入框的文本，当启用此变量时，将直接从主输入框匹配文本

插值使用示例

![UTOOLS1556780752100.png](https://i.loli.net/2019/05/02/5cca96d32ea14.png)

![UTOOLS1556780846840.png](https://i.loli.net/2019/05/02/5cca973294933.png)

## 下载

[百度网盘](https://pan.baidu.com/s/1kEEQcQ1p3Rjli2sTtmCcTg) 提取码: `rbek`

[项目地址](https://github.com/fofolee/uTools-QuickerCommand)

[插件发布页](https://yuanliao.info/d/424)

## 安装方法

将`upx`文件拖入`uTools`输入框中安装即可

## 关键字

`快捷命令` `QuickCommand`

## 鸣谢

鸣谢`uTools`团队，插件中使用的`robotJS`使用的是`剪贴板`插件中的`robotJS`，省去了自行编译的麻烦，在此感谢！

## 另：两个小需求

希望插件的`Features`能够支持以`base64`作为图标，好实现多设备的图标同步，目前的实现方案有点麻烦~
另外可以根据使用的操作系统动态启用或禁用某些`Feature`，即给`Feature`添加类似`platform`的功能