# 我的技术博客

一个基于 Hexo 的个人技术博客，用于分享前端开发技术知识和学习心得。

## 博客简介

- **主题**: 使用 Pure 主题
- **功能**: 支持标签分类、文章归档、代码高亮等
- **内容**: 主要分享前端开发相关技术知识

## 快速开始

### 环境要求

- [Node.js](https://nodejs.org/)
- [pnpm](https://pnpm.io/)
- [Git](https://git-scm.com/)

### 安装步骤

1. 克隆仓库

```bash
# 克隆仓库
https://github.com/lwy-git/lwy-git.github.io.git
cd my_Blog
```

2. 安装依赖

```bash
# 使用pnpm安装依赖
pnpm install
```

3. 本地预览

```bash
# 启动本地服务器
pnpm run server
# 或
pnpm run dev
```

博客将运行在 http://localhost:4000

## 命令说明

```bash
# 清理生成的文件
pnpm run clean

# 生成静态文件
pnpm run build

# 部署到远程仓库
pnpm run deploy

# 启动本地服务器
pnpm run server
```

## 目录结构

```
my_Blog/
├── .deploy_git/       # 部署相关文件
├── public/            # 生成的静态文件
├── scaffolds/         # 模板文件
├── source/            # 源码目录
│   ├── _posts/        # 文章目录
│   ├── about/         # 关于页面
│   ├── categories/    # 分类页面
│   └── tags/          # 标签页面
├── themes/            # 主题目录
│   └── pure/          # Pure主题
├── _config.yml        # 站点配置文件
└── package.json       # 项目依赖配置
```

## 写作指南

### 创建新文章

```bash
pnpm exec hexo new post "文章标题"
```

新文章将创建在 `source/_posts/` 目录下，使用 Markdown 格式编写。

### 文章格式

```markdown
---
title: 文章标题
date: YYYY-MM-DD HH:mm:ss
tags:
  - 标签1
  - 标签2
categories:
  - 分类1
---

# 文章内容

文章正文内容，使用 Markdown 语法编写。
```

### 添加图片

图片应放置在 `source/images/` 目录下，在文章中引用方式如下：

```markdown
![图片描述](/images/图片文件名.jpg)
```

## 配置说明

### 站点配置

主要配置文件为 `_config.yml`，可以修改以下内容：

- 网站标题、描述、作者信息
- 语言设置
- URL设置
- 主题设置
- 部署配置

### 主题配置

主题配置文件为 `themes/pure/_config.yml`，可以修改：
- 导航菜单
- 侧边栏设置
- 颜色方案
- 评论系统
- 分享功能

## 部署指南

### 部署到 GitHub Pages

1. 修改 `_config.yml` 中的部署配置：

```yaml
deploy:
  type: git
  repo: https://github.com/你的用户名/你的用户名.github.io.git
  branch: master
```

2. 执行部署命令：

```bash
pnpm run deploy
```

## 功能特性

- **响应式设计**: 适配不同设备屏幕
- **代码高亮**: 支持多种编程语言的代码高亮
- **标签系统**: 文章支持多标签分类
- **分类系统**: 文章按分类组织
- **文章归档**: 按年月归档文章
- **搜索功能**: 支持站内搜索

## 技术栈

- Hexo: 静态博客生成器
- Pure: 博客主题
- Markdown: 文章编写格式
- Node.js: 运行环境

## 许可协议

本项目采用 [MIT](https://opensource.org/licenses/MIT) 许可证。

## 致谢

- 感谢 Hexo 团队提供的静态博客生成器
- 感谢 Pure 主题的开发者
- 感谢所有支持和访问本博客的朋友

---

欢迎访问我的博客：[https://lwy-git.github.io]
