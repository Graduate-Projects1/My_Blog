## 博客制作

### 方案1：免代码方案 Notion + Vercel (或 Fruition) 搭博客
- 操作方式：
  - 用 Notion 写简历、笔记等内容
  - 用 Fruition 或 NotionNext 把 Notion 页面变成博客网站
  - 用 Vercel 免费部署
- 优点：完全免代码，免费，支持 Markdown，界面美观，SEO 支持
- 适合你展示：个人简历、技术笔记、生活图文、图片展示（Notion 支持图床）

### 方案2：轻代码方案 Next.js + Tailwind CSS + Notion API
- 用 React 框架的 Next.js 搭配 Tailwind CSS 构建前端
- 内容从 Notion 自动抓取展示
- 可部署到 Vercel，拥有顶级响应速度与 SEO

#### 📚 需要补充的知识（可按需学）
| 内容            | 用途            | 推荐学习方式                                    |
| ------------- | ------------- | ----------------------------------------- |
| Markdown      | 写博客笔记、简历      | 半小时掌握：[MarkDown 教程](https://markdown.tw/) |
| Git / GitHub  | 托管代码、博客内容     | B站 / 廖雪峰的教程                               |
| HTML + CSS 基础 | 理解网页结构和样式     | MDN / 菜鸟教程 / B站入门视频                       |
| 前端框架（选学）      | React / Vue   | 适合深入后学习                                   |
| 图片管理          | 上传图片到图床显示在博客中 | sm.ms / imgur / GitHub 图床                 |

### 📌 总结推荐（快速启动）
| 目标         | 推荐方案                        |
| ---------- | --------------------------- |
| 不懂代码但想快速搭建 | Notion + Fruition / Vercel  |
| 能学一点代码，想定制 | GitHub Pages + Jekyll/Hexo  |
| 想未来长期维护扩展  | Next.js + Tailwind CSS（需学习） |
