# 三件好事 · Three Good Things

> 每天记下三件好事，慢慢看见生活里的光。

一个「三件好事」记录 App。想法来自积极心理学里经典的感恩练习 **Three Good Things**（Seligman）：每天睡前写下当天发生的三件好事，并简单说明它为什么让你开心。

**当前状态**：已定 Web 形态 + 静态原型（v0.1），接下来用 Vue 3 工程化实现。

## 原型

静态原型在 [`docs/index.html`](docs/index.html)，**双击用浏览器打开**即可（页面按手机宽度设计，桌面端会显示手机外壳）。

![界面预览](docs/preview-today.png)

| 页面 | 说明 |
| --- | --- |
| [今天（空）](docs/preview-today.png) | 默认打开就能写，填 1 条就能保存 |
| [今天（填了）](docs/preview-filled.png) | "为什么它让你开心" 展开状态 |
| [回顾](docs/preview-review.png) | 日历点亮 + 随机翻一条 |
| [我的](docs/preview-mine.png) | 提醒、导出、清空数据 |

## 已定的选择

- 形态：**Web（H5）**，不做小程序；以后要小程序可以用 uni-app 迁大部分 Vue 代码
- 前端：**Vue 3 + Vite + TypeScript**，CSS 手写（不引 UI 库）
- 首版存储：**localStorage** + 导出 JSON / Markdown，先不做账号
- 后端：**Go**，第二版再加（接口按 REST 设计，存储层会单独抽象）
- 风格：暖色手账感（暖白 `#FAF6F0`、主色 `#D97742`）

## 功能草案

| 版本 | 功能 |
| --- | --- |
| MVP | 今天写 1–3 条 + 可选"为什么"；按日时间线；日历回顾；导出；本地存储 |
| 第 2 版 | 随机回顾 / 那年今日；统计；标签；PWA 提醒；深色模式 |
| 第 3 版 | Go 后端 + 账号同步；年度好事报告 |

## 目录结构

```
docs/
  index.html        静态原型（v0.1）
  preview-*.png     原型截图
  design.md         产品构思、待决问题、里程碑
```

## 开发

技术栈确定后补充（Vue 工程化）。

## 许可

[MIT](LICENSE)
