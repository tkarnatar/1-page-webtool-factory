# 🚀 MicroTool Promo Factory (单页网页工具矩阵生成系统)

这是一套专为 **「工程即营销（Side Project Marketing）」** 打造的自动化单页网页工具生产系统。通过提供 100% 免费、免登录、纯前端运行的实用微工具，吸引搜索引擎与社交媒体的精准流量，并在页面中原生嵌入你其他主力项目的广告、截图与转化链接。

---

## 📁 目录结构

```text
1 page webtool/
├── 📄 promo-config.json         # 你的主力项目推广配置（修改这里的文案、截图与链接）
├── 📄 AI_AGENT_PROMPT.md        # 供 Google Drive 另一台电脑 AI 自动化生产的指令手册
├── 📁 templates/
│   └── 📄 single-tool-template.html # 基础标准单页骨架 (带广告位与SEO)
├── 📁 tools/                    # 已经生成好的开箱即用范例工具
│   └── 📁 kerning-tester/       # 范例: 交互式字体字距 (Kerning) 测验工具
│       └── 📄 index.html
└── 📁 output/                   # 存放未来 AI 自动批量产出的新工具
```

---

## 💻 如何同步到 Google Drive 并让另一台电脑的 AI 制作？

1. **第一步：同步到 Google Drive**
   - 直接把当前整个 `1 page webtool` 文件夹拖入你的 **Google Drive** 或 Google 云端硬盘同步目录。
2. **第二步：配置你的主力项目广告**
   - 打开 [promo-config.json](file:///c:/Users/Matrixkuo/Desktop/Antigravity/APP%20Design/1%20page%20webtool/promo-config.json)，把里面的 `name`, `targetUrl`, `screenshotUrl`, `description` 换成你真实项目的宣传图与链接。
3. **第三步：在另一台电脑上吩咐 AI**
   - 另一台电脑的 AI（如 Antigravity / Cursor / Claude / ChatGPT）读取到 Google Drive 中的文件后，你直接发一句话：
   > *"请阅读 AI_AGENT_PROMPT.md 和 promo-config.json，帮我制作一个 [CSS 阴影生成器] 单页工具，输出到 output/css-box-shadow/index.html"*
4. **第四步：免费上线部署**
   - 产出的 `index.html` 无需任何服务器环境，直接丢到 **Cloudflare Pages**、**GitHub Pages** 或 **Vercel**，绑定你的域名即可秒级上线！
