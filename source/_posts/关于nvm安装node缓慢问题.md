---
title: 关于nvm安装node缓慢问题
date: 2024-05-31 11:29:59
tags:
---

### 出现场景
``` node
$ nvm intsall [node version]
```

### 异常
``` text
大致是什么地址未找到,timeOut!
```

### 解决方案
``` bash
$ where nvm
# 找到对应的目录下的settings.txt
# 设置npm_mirror:
nvm npm_mirror: https://npmmirror.com/mirrors/npm/
# 设置node_mirror:
nvm node_mirror: https://npmmirror.com/mirrors/node/
```

