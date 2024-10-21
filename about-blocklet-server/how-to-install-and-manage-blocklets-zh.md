# How to install and manage blocklets on Blocklet Server

这一节，我们会对着实际的页面进行演示下面的基本动作：

- https://node-dev-1.arcblock.io/admin/blocklets

## Install

我们只要有一个符合 blocklet 规范的 url 路径，就可以把一个 blocklet 安装到 blocklet server，不管这个路径是本地文件还是任何链接。但是绝大部分情况我们都是从 blocklet store 直接安装 blocklet 到 blocklet server。

## Run / Stop / Update

我们可以在 blocklet 中管理每个 blocklet 的运行、停止、更新

## Backup

这里是利用了 DID Space 这个 Blocklet 的能力，去把 blocklets 的数据储存到某一个 DID Space 中，我们一般会用 arcblock 部署的 DID Space 去存储。

## Delete

删除就是把 blocklet 从 server 中移除，删除的时候可以选择保留数据还是移除数据。
