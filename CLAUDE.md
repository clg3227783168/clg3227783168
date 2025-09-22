# CLAUDE.md

## 项目概述

这是一个基于Hugo的静态网站项目，使用hugo-theme-stack主题。网站是Leo Chen的个人站点。

## 核心架构

- **静态站点生成器**: Hugo
- **主题**: hugo-theme-stack (作为git submodule)
- **部署**: GitHub Pages (通过GitHub Actions自动部署)
- **内容结构**:
  - `content/` - 网站内容，包括灵感(inspiration)、待办事项(todo)、解决方案(solution)等页面
  - `layouts/` - 自定义布局模板
  - `themes/hugo-theme-stack/` - 主题文件(git submodule)
  - `static/` - 静态资源文件

### 部署
项目使用GitHub Actions自动部署到GitHub Pages。推送到main分支时会自动触发构建和部署。

## 配置文件

- `hugo.toml` - Hugo主配置文件，包含网站基本信息、菜单配置、评论系统(giscus)配置
- `.github/workflows/hugo.yaml` - GitHub Actions工作流，用于自动构建和部署
- `.gitmodules` - Git子模块配置，包含hugo-theme-stack主题

## 重要注意事项

1. 主题以git submodule方式管理，修改主题时需要注意子模块更新
2. 网站语言设置为中文(zh-CN)
3. 评论系统使用giscus，已配置相关参数
4. 部署的baseURL为 https://clg3227783168.github.io/

## 内容管理

- 新建文章放在 `content/posts/` 目录下
- 页面分为多个部分：灵感、待办事项、解决方案
- 支持分类和标签功能