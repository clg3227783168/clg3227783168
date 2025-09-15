---
title: "解决 Marp 中文 PDF 导出问题"
date: 2025-09-15
tags: ["Marp", "Hugo", "字体"]
categories: ["技术教程"]
---

## 问题描述

使用 Marp for VS Code 将 Markdown 转换为 PDF 时，中文字体无法正常显示。

## 解决方法

安装 `noto-cjk` 字体库。

```bash
sudo apt-get install fonts-noto-cjk
```
