# Claude Code 入门使用指南

> Claude Code 是 Anthropic 官方推出的命令行界面 AI 编程助手，能够直接在你的终端中帮助你分析代码、编写功能、修复 Bug 等。本文记录我的入门体验和基本使用方法。

---

## 📋 什么是 Claude Code

Claude Code 是 Anthropic 发布的 **CLI 工具**，让你可以在终端中直接与 Claude 大模型交互。它的特点：

- 🔌 **直接访问你的代码库** - Claude 可以读取你的文件，理解项目结构
- 🛠️ **自动执行修改** - 可以直接帮你编辑文件，甚至运行命令
- 🧠 **支持上下文窗口大** - Claude 3.5/4 系列模型支持超大上下文
- 🔒 **本地安全** - 代码只在你的机器上处理，API 传输加密

## 🚀 安装

### 前置条件

- 需要有 [Anthropic API](https://console.anthropic.com/) 密钥
- Node.js 18+ 环境

### 安装命令

```bash
npm install -g @anthropic-ai/claude-code
```

或者使用 npm 全局安装：

```bash
# 验证安装
claude --version
```

### 配置 API Key

```bash
# 设置环境变量（添加到 ~/.bashrc 或 ~/.zshrc）
export ANTHROPIC_API_KEY=your-api-key-here
```

## 💡 基本使用

### 启动 Claude Code

在你的项目目录下直接运行：

```bash
claude
```

进入交互模式后，你就可以直接提问了。

### 常用场景

#### 1. 分析现有代码

```
你能帮我分析一下这个项目的目录结构，主要功能是什么吗？
```

#### 2. 修复 Bug

```
这个函数有个 bug，当输入为空的时候会报错，帮我看看并修复它。
```

#### 3. 新增功能

```
帮我在这个文件里新增一个功能，实现 xxx 功能。
```

#### 4. 代码重构

```
帮我重构这段代码，让它更清晰易维护。
```

### 常用快捷键/命令

- `/help` - 查看帮助
- `/exit` - 退出
- `/clear` - 清空上下文
- `/compact` - 压缩上下文，节省 token

## ✨ 我的使用技巧

### 1. 给 Claude 明确的上下文

> **不好**："帮我看看这个项目"
>
> **好**："这是一个 Node.js 后端项目，使用 Express 框架。我现在需要在 userController.js 里新增一个获取用户列表的接口，请帮我完成"

### 2. 善用 Git 集成

Claude Code 会自动检测你项目的 Git 状态，在修改前会帮你查看差异。接受修改后，可以直接在 Claude 中提交。

### 3. 控制修改范围

如果你只希望 Claude 修改特定文件，可以明确指定：

```
只修改 src/utils.js 文件，不要碰其他文件。
```

## ⚠️ 注意事项

1. **Token 消耗**：大上下文会消耗更多 token，注意监控你的 API 用量
2. **代码审查**：Claude 写出的代码一定要自己检查后再合并
3. **敏感信息**：不要把 API Key、密码等敏感信息放到 Claude 上下文中
4. **网络**：国内使用需要配置好代理

## 📝 总结

Claude Code 是目前体验最好的 AI 编程辅助工具之一，特别是对于喜欢在终端工作的开发者来说非常顺手。它的最大优势在于：

- 官方模型，质量有保障
- 能够直接操作文件和执行命令
- 大上下文窗口适合分析整个项目

后续我会继续分享更多 Claude Code 的高级使用技巧。

---

**下一篇：** [Claude Code 进阶技巧](/md/claude-code/advanced-tips.md) - 待更新
