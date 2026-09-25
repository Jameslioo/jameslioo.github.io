# James 的博客

简洁的 Jekyll 博客，使用 GitHub Pages 默认构建，无需第三方主题或插件。

## 上线

将本目录内全部文件放在 jameslioo.github.io 仓库的根目录。不要将 james-blog 外层文件夹上传，也不要只上传 ZIP。

在仓库 Settings → Pages 中设置：Source 为 Deploy from a branch，Branch 为 main，Folder 为 /(root)，点击 Save。等待 Actions 中部署完成后访问 https://jameslioo.github.io/ 。

## 文件分工

- `_config.yml`：博客名称、介绍、网址。
- `_posts/`：Markdown 文章。
- `_layouts/`：网页与文章模板。
- `_includes/archive.html`：按年份自动生成文章列表。
- `assets/style.css`：颜色、字体、间距及手机布局。
- `about.md`：个人介绍。

## 写文章

在 `_posts/` 新建 `YYYY-MM-DD-英文短名.md`，例如 `2026-09-26-first-note.md`：

```markdown
---
layout: post
title: "我的第一篇学习笔记"
---

在这里写正文。
```

日期不能晚于当前时间，否则 Jekyll 默认不发布。文章发布后尽量不改文件名，以免链接变化。

将图片放进 `assets/images/`，正文使用 `![图片说明](/assets/images/example.png)` 引用。

改动后提交并推送，GitHub Pages 自动重建。归档列表不需要手动维护。

示例文章与关于页面是占位内容，请替换成自己的文字。本模板不包含评论、账号后台或数学公式渲染；需要时再添加。
