# ChangeLog
## v0.4.0: 21/05/21
- `feat`: 添加对`mpnews`类型消息的支持，关于该类型的解释参考[官网](https://work.weixin.qq.com/api/doc/90000/90135/90236#%E5%9B%BE%E6%96%87%E6%B6%88%E6%81%AF%EF%BC%88mpnews%EF%BC%89)
- `feat`: 添加对参数`enable_id_trans`, `enable_duplicate_check`,`duplicate_check_interval`，现在你可以在发送消息的时候指定它们，具体参考官网
- `refactor`: 更改参数`safe`为`int`，含义与官网等同，优化部分代码

## v0.3.1: 21/05/17
- `fix`: 修复不同企业同一id应用的token存储冲突问题
## v0.3.0: 21/05/16
-  `feat`: 支持在同一个项目中创建多个应用消息推送

## v0.2.4: 21/05/11
- `fix`：修复因单例模式参数设置不正确导致实例化`AppMsgSender`异常的问题
- `v0.2.1`特性继承
- `v0.2.2`特性继承
- `v0.2.3`特性继承

## ~~v0.2.3: 21/05/10~~
- `fix`: 修复从`pypi`安装`corpwechatbot`出现的找不到`pypidoc.md`的错误

## ~~v0.2.2: 21/05/07~~

- `fix`: 1000004
- `refactor`: 优化重构`AppMsgSender`部分代码，更改传参机制
- `docs`: 更新使用文档和README文档的内容

## ~~v0.2.1: 21/04/24~~
- `fix`: 修复终端直接运行-u参数随意输入报错的问题
- `feat`: 现在支持在发送`markdown`信息的时候直接传入`markdown`文件路径
- `docs`: 添加专用用于`pypi`的文档
- `docs`: 添加为何使用`corpwechatbot`的文档说明到`README`

## v0.2.0: 21/04/18
- `feat`: 允许在本地创建文件读取企业微信配置，避免每次程序都要传入
- `feat`: 支持在命令行直接执行包发送信息，如`cwb -u='app' -t='hello world'`
- `fix`：token存储位置修改，初始设置保存到本地`site-packages`（后期将其移到`site-packages/corpwechatbot`目录下，方便统一）

## v0.1.0: 21/04/09
- 项目初始化建立
- 添加群聊机器人消息推送
- 添加应用消息推送，暂不支持**小程序消息、任务卡片消息**