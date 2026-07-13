<!-- ============================================
     OWD.K-MD3 首页小组件定义
     每个 widget 是一个独立的展示单元
     通过 Grid Areas 布局排列
   ============================================ -->

<!--
  桌面端布局: 三列
  featured 占满首行，下面 stats + news 并排，再下面 links 占满
-->
<!-- areas:desktop="featured featured featured" "stats news versions" "links links links" -->

<!-- 平板端: 两列 -->
<!-- areas:tablet="featured featured" "news stats" "versions versions" "links links" -->

<!-- 手机端: 单列 -->
<!-- areas:mobile="featured" "news" "stats" "versions" "links" -->


<!-- widget:area=featured,type=featured,color=primary -->
## 欢迎来到 OWD.K-MD3
基于 Material Design 3 的轻量级文档站点框架。零构建工具，纯前端实现，只需编写 Markdown 文件即可拥有现代化文档网站。

支持亮色/暗色双主题，响应式布局，JSON 配置驱动。严格遵循 MD3 设计规范，精致视觉层次与动效。
[开始阅读](page/)
<!-- /widget -->


<!-- widget:area=news,type=news,color=secondary -->
## 最新动态
### 2026-07-13
新增小组件系统，首页展示更灵活
### 2026-07-10
CSS Grid Areas 自由布局能力上线
### 2026-07-01
OWD.K-MD3 框架首个版本发布
### 2026-06-25
文档页主题切换功能完成
[更多动态](page/#/)
<!-- /widget -->


<!-- widget:area=stats,type=stats,color=tertiary -->
## 项目统计
| 指标 | 数值 |
|------|------|
| 文档页数 | 3 |
| 配置项 | 20+ |
| 内置主题 | 2 |
| CSS 变量 | 60+ |
| 组件类型 | 8 |
<!-- /widget -->


<!-- widget:area=versions,type=versions,color=neutral -->
## 平台版本
| 平台 | 版本 |
|------|------|
| Web | v2.0 |
| PWA | v2.0 |
| 离线包 | v1.5 |
<!-- /widget -->


<!-- widget:area=links,type=links,color=primary -->
## 快速入口
- [文档首页](page/)
- [配置指南](page/#/guide)
- [GitHub](https://github.com)
- [更新日志](page/#/)
- [反馈问题](https://github.com)
<!-- /widget -->
