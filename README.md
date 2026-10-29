# 我的 Hexo 博客

博客地址：https://joe419476-cell.github.io/

源码仓库：https://github.com/joe419476-cell/joe419476-cell.github.io

使用 Hexo 和 Landscape 主题。推送到 main 分支后，GitHub Actions 自动构建并发布到 GitHub Pages。

## 本地预览

安装 Node.js 22 和 Git，在本项目目录执行：

```bash
npm ci
npm run server
```

打开 http://localhost:4000 。按 Ctrl+C 停止预览。Windows 如果不允许执行 npm.ps1，可将 npm 替换为 npm.cmd。

## 写文章

```bash
npm run new -- "我的第一篇文章"
```

编辑 source/_posts/ 下对应的 Markdown 文件。文件开头的 title、date、tags 和 categories 分别是标题、发布日期、标签和分类。默认不显示未来日期的文章；时区是 Asia/Shanghai。

文章中插入 <!-- more --> 可设置首页摘要的结束位置。

## 发布更新

```bash
git add .
git commit -m "Update blog"
git push
```

在仓库的 Actions 页面查看部署结果。发布源应为 Settings → Pages → Source → GitHub Actions。工作流使用 GitHub 自带令牌，无需另建个人访问令牌。

## 修改信息

- _config.yml：博客标题、副标题、作者、网站地址。
- _config.landscape.yml：菜单、侧栏、GitHub 链接。
- source/about/index.md：个人介绍。
- source/_posts/：文章。

本地检查构建：npm run build。需要清理缓存时运行 npm run clean。

node_modules/、public/ 和生成缓存无需提交；package-lock.json 应随源码提交。

官方文档：[Hexo 写作](https://hexo.io/docs/writing.html)、[GitHub Pages 部署](https://hexo.io/docs/github-pages.html)。
