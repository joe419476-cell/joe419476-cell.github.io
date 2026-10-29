---
title: 你好，世界
date: 2026-10-29 08:00:00
tags:
  - Hexo
categories:
  - 博客搭建
---

欢迎来到我的博客！这里将记录学习过程、技术笔记与生活中的小发现。

<!-- more -->

## 写下第一篇文章

在博客项目目录打开终端，运行：

```bash
npm run new -- "我的第一篇文章"
```

编辑 `source/_posts/` 下新生成的 Markdown 文件，然后在本地预览：

```bash
npm run server
```

打开 http://localhost:4000 查看效果。文章开头的 `title`、`date`、`tags` 和 `categories` 分别控制标题、日期、标签和分类。

## 发布更新

将修改提交并推送至 GitHub 的 `main` 分支，GitHub Actions 会构建博客并部署到 GitHub Pages。

愿每一次记录，都成为下一次进步的起点。
