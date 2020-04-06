# 目录结构

| 目录名 | 详情/解释 |
| :--- | :--- |
| **property.js** | 控制面板配置文件 |
| **core/logo.txt**               | 控制台输出 logo 文字 |
| **public/** | 前端所有代码，资源目录，前后端分离，使用 ws 和 ajax 通讯 |
| **public/login/**               | 纯 UI 逻辑登陆页面 |
| **public/template/**             | 前端业务模板，每个模板拥有着一个生命周期，开始与结束。 |
| **public/onlinefs\_public/**       | 文件在线管理模块前端所有代码 |
| **public/common/js/meum.js** | 控制面板左侧菜单列表 |
| **public/common/js/login.js** | 通用登录流程逻辑，可重复利用在各类 HTML 登录模板 |
| **server/server\_core**           | Minecraft 服务端核心目录，包括服务端文件，配置，Mod，以及插件 |
| **server/x.json**               | Minecraft 服务器面板配置文件 |
| **users/x.json**               | 控制面板用户配置文件 |
| **route/**                     | 控制器，HTTP 请求业务逻辑层（可二次扩展） |
| **route/websocket/**             | 控制器，Webscoket 请求业务逻辑层（可二次扩展） |
| **core/Process/**               | Minecraft Server 类实现 |
| **core/User/**                   | User 类实现 |
| **core/DataModel.js**             | 数据持久化模型，几乎是所有的配置的 I/O 模型 |
| **model/**                     | 模型层，用于提供控制器与服务端，用户操作，也提供设计模式模型 |
| **helper/**                     | 业务逻辑辅助层，用于辅助和重复利用业务逻辑 |
| **ftpd/**                       | FTP 独立模块，其中 ftpserver.js 已经实现了抽象 ftpServerInterface 接口 |
| **onlinefs/**                     | 文件管理独立模块 \([Suwings/IndependentFileManager](https://github.com/Suwings/IndependentFileManager)\) |

### ~~**注意：由于MDUI的部分组件在PJAX下无法正常发挥，所以我无奈之下复制粘贴了Github的表格。。。。**~~

#### **忽略这一段话，gitbook赛高**

