# 水手辛巴德的 AI 笔记

个人技术博客，记录 AI 时代下的编程学习与实践经验。

- 📝 博客地址：https://chengzhixuancode.github.io
- 💡 理念：用长期的确定性，对抗短期的不确定性

## 技术栈

- [docsify](https://docsify.js.org/) - 静态文档网站生成器
- GitHub Pages - 托管

## 项目结构

```
chengzhixuancode.github.io/
├── docs/                # 网站根目录
│   ├── _coverpage.md    # 封面页
│   ├── _sidebar.md     # 侧边导航
│   ├── index.html       # 入口 HTML
│   └── md/             # 文章内容按分类存放
│       ├── claude-code/  # Claude Code 相关文章
│       └── openclaw/    # OpenClaw 相关文章
├── LICENSE
└── README.md
```

## 内容分类

- 🤖 AI 编程工具实践（Claude Code、OpenClaw 等）
- 💡 AI 辅助开发经验总结
- 🔧 提示工程技巧
- 🚀 AI 项目实战

## 常用命令

本项目是纯静态 markdown 文档站点，无需构建：

- 本地预览：`npx docsify serve docs`
- 部署：推送到 GitHub 即可，GitHub Pages 自动托管

## 开发指南

- 所有文章都是 markdown 格式，存放于 `docs/md/{category}/` 目录
- 添加新文章后需要更新 `docs/_sidebar.md` 导航
- 遵循现有文章的格式风格，使用一级标题作为标题，二级标题分隔章节
