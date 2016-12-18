---
title: 团队打包流程与规范
layout: page
permalink: "/packaging/"
---

## 团队打包指南

### 添加一个软件包

如果你想要将 Debian 中已有的一个软件包置于中文开发者团队旗下进行维护，
请向[团队 Alioth 邮件列表](mailto:chinese-developers@lists.alioth.debian.org)
发送邮件并解释原因。

如果你找到了一个尚未打包的有趣软件，而且你想将其置于中文开发者团队下进行维护，
请先按照标准的 ITP 流程进行工作。同时，请向我们的邮件列表发送一封邮件阐述你的打算。

#### 接受标准

团队一般会接受与中文、中文使用者、大中华地区相关的软件包。
如果你不确定某个软件包是否满足情况，请与我们取得联系。

### 维护软件包

#### 工作流

我们使用 Git 管理团队软件包。建议按照 [DEP-14](http://dep.debian.net/deps/dep14/)
的流程要求管理并统一 Git 仓库结构。

* [团队 Git 仓库一览](https://anonscm.debian.org/git/chinese/)

#### 规则与提醒

* 如需建立新的 Git 仓库，请考虑使用 Alioth 主机上的对应脚本来自动生成；
* Git 标签必须使用**annotated tags**。这个要求由 Git 钩子所强制检查。
* 无法使用 Git 命令移除远程标签，所以操作请小心。如果有差错，只能远程登录 Alioth 主机进行操作。
* 所有新提交会触发向 [chinese-commits](mailto:chinese-commits@lists.alioth.debian.org) 发送邮件。这个要求由 Git 钩子所实现。
* 请多多与团队成员进行交流沟通。如果需要对他人维护的团队软件包进行修改，最好在邮件列表中预先知会对方。
