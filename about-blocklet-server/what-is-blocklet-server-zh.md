# 什么是 Blocklet Server？

## 什么是 Blocklet？

首先， blocklet 是我们公司对应用的称呼，理论上它可以是任何应用（现在大部分是 nodejs 应用），最终它会运行在 Blocklet Server 上。

比较直观的理解：Pages-Kit 是一个 Blocklet，AIGNE 也是一个 Blocklet，基本上公司的产品除了 Blocklet Server 和 DID 之外，都是 Blocklet。

Blocklet Server 是 Blocklet 的运行环境，是 Blocklet 的运行平台。每个 Blocklet 的生命周期都由 Blocklet Server 管理。

## Blocklet Server 的基本架构图

Blocklet Server 是基于 nodejs 开发的，我们大部分 Blocklet 也是基于 nodejs 开发的。

Blocklet Server 内部还分为两块：Blocklet Server 和 Blocklet Service。

每个 Blocklet 都会被 Blocklet Service 包裹，从中获得一些基本能力，比如登录、数据存储、消息推送等。

比较直观的架构图（我们现在先不仔细阅读它）：

https://team.arcblock.io/comment/docs/c158aee4-accd-42f4-9ced-6a23f28c00e0/en/L0P8cWeYx15c1GB_4Tnk_TFv#a6045171-3e58-4717-84bf-2d08a2684a58

## Blocklet Server 的用户结构

一个完整的 Blocklet Server 应该有三层用户：

- 平台运行方，提供 Blocklet Server 运行环境，让其他用户可以来这个平台购买和部署 Blocklet， arcblock.io 就是一个平台运行方，当然任何人都可以利用 Blocklet Server 搭建自己的平台
- Blocklet 的 Owner，这是平台运行放的直接用户，他们在平台上购买空间，然后部署自己的 Blocklet (这是我们公司未来的主要用户)
- Blocklet 的 User，这是 Blocklet Owner 的客户，他们使用 Blocklet （有的时候 Blocklet 的 Owner 和 User 是同一个人，比如说有人自己部署一个 discuss-kit 自己用）

还有一类特殊的用户：

- Blocklet 开发者，这类用户开发自己的 Blocklet 发布到 Blocklet Store 上，赚取收益。现在还没有特别严肃的外部 Blocklet 开发者，基本上都是我们公司的员工。
