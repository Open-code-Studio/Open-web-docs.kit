# Project Memory - Open-web-docs.kit (OWD.K-MD3)

## 项目概览
基于 Material Design 3 的轻量级文档站点框架，纯前端实现（零构建工具），通过 `page/config.json` 配置驱动。

## 文件结构
- `index.html` - 首页/主界面（Hero + Features + Widgets + Nav Cards + Links + Footer）
- `page/index.html` - 文档阅读页（Sidebar + TOC + Markdown 渲染）
- `page/config.json` - 站点配置（site/nav/sidebarLinks/home）
- `page/js/app.js` - 文档页核心逻辑（214行，IIFE 模式）
- `page/css/theme.css` - MD3 主题令牌（亮色/暗色）
- `page/css/layout.css` - 文档页布局
- `page/css/components.css` - UI 组件样式
- `page/css/markdown.css` - Markdown 渲染样式
- `page/css/home.css` - 首页专属样式
- `docs/_widgets.md` - 首页小组件定义（Grid Areas 布局 + 5 种 widget 类型）
- `docs/` - Markdown 源文件

## 关键设计决策
- config.json 的 `home` 字段仅被首页使用，文档页的 app.js 通过 `Object.assign` 只读取 `site/nav/sidebarLinks`，完全向后兼容
- 首页和文档页各自独立管理主题（localStorage key 分别为 `owd-home-theme` 和 `theme`），互不干扰
- 首页导航卡片的链接格式：`page/#/` + 页面 slug
- 小组件系统使用 CSS Grid Areas 命名区域布局，`matchMedia` 自适应桌面/平板/手机三档断点
- 小组件定义格式：`<!-- widget:area=NAME,type=TYPE,color=COLOR -->` + Markdown 内容 + `<!-- /widget -->`
- 支持五种 widget 类型：featured、news、stats、versions、links，每种有独立视觉样式
