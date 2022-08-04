# Tailchat

Tailchat 是一款现代化开源的即时通讯聊天应用，基于 React + Typescript 开发

前端微内核架构+后端微服务架构，Tailchat 已经为集群化部署做好了准备。

前端通过插件机制为应用赋能，对于 Tailchat 的二次开发来说非常简单且易用。

官方文档: [https://tailchat.msgbyte.com/](https://tailchat.msgbyte.com/)

后端仓库地址: [tailchat-server](https://github.com/msgbyte/tailchat-server)

Nightly版 体验地址: [https://nightly.paw.msgbyte.com/](https://nightly.paw.msgbyte.com/)

> Nightly版 为自动编译版本, 即每次提交代码都会自动编译。
> 不保证数据的可靠性与稳定性 

**NOTICE: 虽然目前Tailchat的核心功能处于稳定阶段，但它对于第三方开发者暴露的接口仍在不断完善中，一般来说是向下兼容的，但保留出现 Break Change的可能性**

## Feature

- 注重隐私，只有被邀请的成员才能加入群组
- 防止陌生人，只有通过昵称+一串随机的数字才能添加好友
- 二维的群组空间，通过频道来分割不同的话题
- 高度自定义的群组空间, 通过分组和拖拽来创建独创的群组空间。同时可以通过更多的插件来增加更多的能力
- 可以严谨，也可以乐趣。通过插件的组合可以创造用于不同场景的 Tailchat。可以是面向娱乐，也可以是面向企业
- 后端微服务架构，已经为大规模部署做好了准备。不用担心用户量大了以后怎么办


## Build

#### 编译 web 前端代码

```bash
pnpm install
cd web
SERVICE_URL=http://127.0.0.1:11000 pnpm build
```

环境变量: 
- `SERVICE_URL`: 后端服务的地址

使用任意方式代理 `web/dist` 目录即可。


#### expo 打开移动端app
```bash
cd app
pnpm install
pnpm start
```
