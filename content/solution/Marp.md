---
title: "Marp 导出 PDF 中文乱码"
date: 2025-09-15
tags: ["Marp", "Hugo", "中文乱码"]
categories: ["bug解决"]
---

## 问题描述

使用 Marp for VS Code 将 Markdown 转换为 PDF 时，中文字体无法正常显示。

## 解决方法

安装 `noto-cjk` 字体库。

```bash
sudo apt-get install fonts-noto-cjk
```
