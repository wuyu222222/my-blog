<div align="center">

# ✨ Hexo Theme Frutiger Aero

一款怀旧风格的 Hexo 主题，灵感源自 2000 年代中后期到 2010 年代初期的 Frutiger Aero 审美

[English](./README_EN.md) | 简体中文

</div>

![预览图](./screenshot.png)

## 🎨 特性

<table>
  <tr>
    <td width="50%">
      <h4>🪟 拟物化玻璃效果</h4>
      <p>利用 <code>backdrop-filter</code> 实现高质量的毛玻璃拟态</p>
    </td>
    <td width="50%">
      <h4>🌈 鲜艳渐变色</h4>
      <p>采用该时代典型的亮蓝色与绿色配色方案</p>
    </td>
  </tr>
  <tr>
    <td width="50%">
      <h4>🫧 动态气泡</h4>
      <p>背景中漂浮的 CSS 动画气泡，增强怀旧氛围</p>
    </td>
    <td width="50%">
      <h4>📱 响应式设计</h4>
      <p>完美适配手机、平板及桌面端</p>
    </td>
  </tr>
  <tr>
    <td width="50%">
      <h4>⚡ 轻量快捷</h4>
      <p>无沉重依赖，加载速度快</p>
    </td>
    <td width="50%">
      <h4>🎮 特色功能</h4>
      <p>内置 Bangumi 追番墙、怀旧时间轴归档及关于页</p>
    </td>
  </tr>
  <tr>
    <td width="50%">
      <h4>📐 侧边栏布局</h4>
      <p>右侧侧边栏展示用户头像、简介、相框和统计信息</p>
    </td>
    <td width="50%">
      <h4>🚀 项目展示页</h4>
      <p>展示你的 GitHub 项目</p>
    </td>
  </tr>
  <tr>
    <td width="50%">
      <h4>📅 自定义日期</h4>
      <p>支持为每篇文章设置自定义发布日期</p>
    </td>
    <td width="50%">
      <h4>💻 代码高亮</h4>
      <p>美化的代码块显示，支持一键复制</p>
    </td>
  </tr>
</table>

## 🚀 快速开始

### 1. 安装

进入你的 Hexo 根目录，克隆本仓库：

```bash
git clone https://github.com/tud8951/hexo-theme-frutiger-aero themes/frutiger-aero
```

### 2. 配置

修改 Hexo 根目录下的 `_config.yml`：

```yaml
theme: frutiger-aero
language: zh-CN
```

### 3. 启动预览

```bash
hexo server
```

## ⚙️ 配置说明

### 完整配置示例

编辑 `themes/frutiger-aero/_config.yml` 来自定义各种功能：

```yaml
# 菜单配置
menu:
  Home: /
  Archives: /archives
  Anime: /anime
  Projects: /projects
  About: /about

# 侧边栏配置
sidebar:
  enabled: true
  username: 你的用户名
  avatar: /img/avatar.png
  description: 热爱生活，热爱技术
  photo_frame: /img/photo.jpg

# 社交链接
social:
  github: 你的GitHub用户名
  twitter: 你的Twitter用户名（可选）

# 追番配置
bangumi:
  enabled: true
  user_id: 你的Bangumi用户ID

# 项目展示配置
# 方式1: 手动配置项目（推荐，不依赖API）
projects:
  - name: 项目名称
    description: 项目描述
    url: 项目链接
    language: 编程语言
    stars: Star数量
    forks: Fork数量
    updated: 更新日期

# 方式2: 从GitHub API获取（可能遇到速率限制）
# github:
#   username: 你的GitHub用户名
#   repos: []
```

### 📐 侧边栏详情

侧边栏包含以下内容：

| 功能 | 说明 |
|------|------|
| 👤 用户信息 | 头像、用户名、个人简介 |
| 🔗 社交链接 | GitHub 和 Twitter 链接 |
| 🖼️ 相框 | 展示一张照片 |
| 📊 站点统计 | 文章、分类、标签数量 |
| 🏷️ 标签云 | 展示所有文章标签 |

### 📅 自定义文章日期

在文章的 front-matter 中可以设置自定义发布日期：

```yaml
---
title: 文章标题
date: 2024-01-01 00:00:00
published: 2025-11-02
tags: [标签1, 标签2]
---
```

### 📁 网站资源

将你的图片资源放入 `source/img/` 目录下：

- `favicon.png` - 网站图标
- `avatar.png` - 用户头像
- `photo.jpg` - 相框图片

## 📄 页面创建

### 🎮 创建追番页面

在 `source/anime/index.md` 中创建：

```markdown
---
title: 追番
layout: anime
---
```

### 🚀 创建项目展示页面

在 `source/projects/index.md` 中创建：

```markdown
---
title: 项目
layout: projects
---
```

## 🤝 贡献

欢迎提交 Issue 和 Pull Request！

## 📄 许可证

MIT License © 2024
