---
title: 入门搭建 Node.js 环境
date: 2020-09-27 21:30:00
---

node 版本管理工具 for  Windows

https://nvm.uihtm.com/

https://github.com/coreybutler/nvm-windows

nvm version                                          // 查看NVM版本

```shell
nvm node_mirror https://npmmirror.com/mirrors/node/ #  设置node阿里云镜像源
nvm npm_mirror https://npmmirror.com/mirrors/npm/ #  设置npm阿里云镜像源
```


nvm list available         // 查看可安装的node版本
nvm list                   // 查看已安装的node版本
nvm install 版本号          // 安装node
nvm uninstall 版本号        // 卸载node
nvm use 版本号              // 切换使用node版本
nvm current                // 当前使用node版本

# 查看 nvm 版本
nvm --version

# 列出所有可安装的 Node.js 版本
nvm list-remote
# Windows 上使用
nvm list available

# 安装最新的 LTS 版本
nvm install --lts

# 安装特定版本
nvm install 18.17.0
nvm install 16.20.1

# 列出已安装的版本
nvm list
# 或
nvm ls

# 切换到特定版本
nvm use 18.17.0

# 设置默认版本
nvm alias default 18.17.0

# 查看当前使用的版本
nvm current

# 卸载特定版本
nvm uninstall 16.20.1

```shell
npm cache clean --force #清除npm缓存
npm config set registry https://registry.npmmirror.com #设置npm源为阿里云镜像源
npm config get registry #查看npm源
```

安装项目依赖
npm install