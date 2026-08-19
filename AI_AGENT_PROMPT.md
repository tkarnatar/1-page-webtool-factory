# 🤖 AI 单页网页工具自动化生产工作流 (AI Agent Workflow SOP)

> **使用说明**：把本文件夹同步至 Google Drive 后，你只需将本文件的指令或需求发给另一台电脑上的 AI（无论是 Claude、GPT、Gemini 或 Antigravity），AI 即可自动按照标准规范生产出高质量、带推广广告、符合 SEO 规范的单页工具。

---

## 🎯 核心使命 (Agent Mission)
你是一位全栈前端开发专家与增长黑客（Growth Engineer）。你的任务是根据给定的**工具功能需求**，自动生产**独立的单页网页工具（Single-Page Web Tool）**。

### 每一个单页工具必须满足以下四大核心法则：
1. **纯前端 / 零成本优先（Client-Side Only）**：
   - 尽可能使用浏览器原生 API（Canvas、Web Audio、SVG、File API）或轻量纯前端开源库（如 `@imgly/background-removal`、`transformers.js`、`fflate`、`jspdf` 等）。
   - 严禁依赖昂贵的付费后端 API，除非用户明确要求。
2. **美学设计高级感（Premium Modern Design）**：
   - 遵循深色质感现代风，字距精致，无杂乱色块，流畅的 Hover 与交互动效。
   - 拒绝土味排版、拒绝无质感的平面色块。
3. **原生广告与高转化导流（Ad & Promo Flywheel）**：
   - 从 `promo-config.json` 中读取推广项目信息，将主力项目的**截图、标题、痛点文案、跳转 CTA 按钮**自然地嵌入在工具界面中（导航栏右侧、操作台下方、结果导出提示）。
4. **内置 SEO 与 FAQ 结构化数据**：
   - 自动生成符合 Google 规范的 Title、Meta Description、OpenGraph 标签以及 2~3 个该工具的高频 FAQ 问答。

---

## 🛠️ 生产标准流程 (Execution Protocol)

### 输入：
用户指定想要的新工具名称或功能描述（例如：`SVG 转 PNG 高清生成器`、`Twitter 推文图片卡片制作器`、`CSS 阴影调试器` 等）。

### 执行步骤：
1. **读取推广配置**：查看 `promo-config.json`，选择最契合该工具属性的主力项目进行引流。
2. **编写完整单文件 `index.html`**：
   - 将所有 CSS、JS 与 HTML 结构完整封装在单个 `index.html` 中（便于零门槛部署）。
3. **输出路径**：
   - 存入 `output/<tool-name>/index.html`（例如 `output/svg-to-png/index.html`）。

---

## 📋 快速触发指令模板 (你可以直接复制给另一台电脑的 AI)

```markdown
请读取当前目录下的 `promo-config.json` 与 `templates/single-tool-template.html`。
我想要生产一个新的单页工具：【在这里输入工具名称与功能，例如：CSS 磨砂玻璃 (Glassmorphism) 实时生成与代码复制器】。

要求：
1. 纯前端实现，开箱即用，支持实时参数调节并一键复制代码。
2. 采用现代极简暗黑高级风 UI，响应式适配手机与电脑。
3. 在工具下方和顶部导航栏嵌入 promo-config.json 中的主力项目推广卡片与截图。
4. 将生成好的完整 HTML 保存至 `output/<工具英文名>/index.html`。
```

---

## 💡 推荐扩充工具清单 (随时可让 AI 生产)

1. **`img-to-webp`**：批量将 PNG/JPG 转换为高压缩率 WebP
2. **`svg-viewer-cleaner`**：SVG 代码实时预览、压缩与清理多余属性
3. **`tweet-card-generator`**：输入文本生成优雅的推特样式分享卡片
4. **`css-glassmorphism`**：CSS 磨砂玻璃实时调节生成器
5. **`app-icon-resizer`**：一键生成 iOS / Android 所有尺寸 App Icon 压缩包
6. **`color-palette-extractor`**：上传图片自动提取 6 种主色调并复制 HEX/RGB
7. **`markdown-to-social-image`**：将 Markdown 文本渲染为高质感长图
