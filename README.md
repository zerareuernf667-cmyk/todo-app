# Todo App

This is my first GitHub project.

## Features
- Basic HTML page
- Todo list

## What I learned
- Git basics
- GitHub workflow
- Pull Request

# 🚀 Git & GitHub 实战入门笔记（完整版）

> 适用于：刚完成第一次完整 GitHub 流程的你
> 目标：巩固 + 可复用 + 可长期参考

---

# 🧠 一、核心理解（必须掌握）

## Git vs GitHub

| 名称     | 作用          |
| ------ | ----------- |
| Git    | 本地版本控制      |
| GitHub | 远程仓库 + 协作平台 |

👉 工作关系：

```
本地代码（Git）
   ↓ git push
远程仓库（GitHub）
```

---

## 四个核心概念

| 概念           | 含义     |
| ------------ | ------ |
| Repository   | 项目     |
| Commit       | 一次版本快照 |
| Branch       | 开发分支   |
| Pull Request | 合并请求   |

---

# ⚙️ 二、本地 Git 操作流程

## 初始化仓库

```bash
git init
```

👉 把当前文件夹变成 Git 仓库

---

## 添加文件

```bash
git add .
```

👉 加入暂存区

---

## 提交代码

```bash
git commit -m "first commit"
```

👉 创建一个版本记录

---

## 查看状态（最重要命令）

```bash
git status
```

👉 随时检查当前状态

---

# 🌐 三、连接 GitHub

## 添加远程仓库

```bash
git remote add origin https://github.com/用户名/仓库名.git
```

---

## 第一次推送

```bash
git push -u origin main
```

👉 建立本地与远程关联

---

## 后续推送

```bash
git push
```

---

# 🌿 四、分支开发（核心技能）

## 创建分支

```bash
git checkout -b feature-xxx
```

---

## 修改 → 提交

```bash
git add .
git commit -m "feat: xxx"
```

---

## 推送分支

```bash
git push -u origin feature-xxx
```

---

# 🔁 五、Pull Request 流程

## 标准流程

```
main（稳定）
   ↓
feature 分支（开发）
   ↓
Push 到 GitHub
   ↓
Pull Request
   ↓
Code Review（可选）
   ↓
Merge
   ↓
回到 main
```

---

## PR 本质

👉 PR = **代码变更提案**

---

# 🔄 六、合并后操作

## 同步本地

```bash
git checkout main
git pull origin main
```

---

## 删除分支

```bash
git branch -d feature-xxx
```

---

# 🔥 七、日常开发标准流程（最重要）

```bash
git checkout main
git pull origin main
git checkout -b feature-xxx

# 开发代码

git add .
git commit -m "feat: xxx"
git push -u origin feature-xxx
```

👉 然后去 GitHub 创建 PR

---

# ⚠️ 八、常见问题 & 解决方案

---

## ❗认证失败

```
Password authentication is not supported
```

👉 原因：GitHub 不支持密码
👉 解决：使用 Token

---

## ❗网络问题

```
Failed to connect to github.com port 443
```

👉 原因：网络限制
👉 解决：

* 手机热点
* VPN / 代理

---

## ❗分支领先

```
ahead of origin/main by 1 commit
```

👉 说明：本地有提交但没 push

---

## ❗push 卡住

👉 可能原因：

* 正在等待输入（终端不显示）
* 网络问题

---

# 🧹 九、良好习惯（非常重要）

---

## ✅ 每次操作前

```bash
git status
```

---

## ✅ 不直接改 main

👉 必须用分支开发

---

## ✅ commit 规范

```
feat: 新功能
fix: 修复 bug
docs: 文档
refactor: 重构
```

---

## ✅ 一个功能一个分支

---

## ✅ 合并后删除分支

---

# 📁 十、项目结构（当前）

```
todo-app/
 ├── index.html
 ├── README.md
 └── .gitignore
```

---

# 🎯 十一、你已经掌握的能力

你现在已经会：

* Git 基础命令
* GitHub 推送
* 分支开发
* Pull Request
* Merge 流程
* 基本排错（网络/认证）

👉 已完成完整入门 ✅

---

# 🚀 十二、下一步学习路线

## 1️⃣ 冲突解决（必学）

```
<<<<<<< HEAD
你的代码
=======
别人代码
>>>>>>> branch
```

👉 学会手动处理

---

## 2️⃣ 项目升级

加入：

* CSS
* JavaScript

---

## 3️⃣ Git 进阶

* rebase vs merge
* squash commit

---

# 🧠 总结一句话

👉 Git = 版本控制
👉 GitHub = 协作平台
👉 分支 + PR = 标准开发流程

---

# ⭐ 建议

👉 把这份文档放到：

* GitHub README
* Notion
* 本地笔记

作为长期参考

---
