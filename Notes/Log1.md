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


## 具体实现：Notion + Next.js + 免费部署
### 🧭 一、整体流程图：Notion 驱动美观博客网站
```css
[内容创作] ➝ [Notion 页面] ➝ [Notion API 连接网站] ➝ [Next.js 网站结构展示] ➝ [Vercel 免费部署上线] ➝ [自定义子域名]
                         ↑
             [Markdown 写简历/笔记/相册页]
```

### 🛠️ 二、具体步骤详解
#### ✅ Step 1：准备内容（简历 / 笔记 / 相册）
- 在 Notion 中建立一个 Workspace 或页面集合，如：
  - /about：个人简介
  - /resume：简历（用表格或文字）
  - /blog：笔记合集（按时间或标签整理）
  - /photos：生活照或图文记事（用图片块+说明文字）
- ✅ 使用 Notion 的“共享链接”设置为公开可访问。

#### ✅ Step 2：搭建前端模板（Next.js + Notion API）
推荐使用开源项目 [NotionNext](https://github.com/tangly1024/NotionNext)：
- 一个用 Next.js 构建的 Notion 驱动博客框架，外观现代，部署简单，维护方便。

##### 🚀 快速搭建步骤：
1. 注册 GitHub 账号
2. Fork 仓库：点击进入 NotionNext
3. 配置 Notion 页面链接
  - 打开仓库的 site.config.js 或 .env 文件
  - 填入你的 Notion 页面 ID（NotionNext 会自动获取页面结构）
4. 部署到 Vercel（免费）
- 登录 Vercel.com → 用 GitHub 授权
- 一键导入你 Fork 的仓库
- 自动部署上线（5分钟完成）

#### ✅ Step 3：个性化设计与修改样式
- 使用 Tailwind CSS（NotionNext 已内建）修改样式：
  - 更改字体、颜色、布局
  - 修改 Logo、导航栏、页脚等

- 你可以从以下文件入手：
  - /config/site.config.js：网站标题、作者名等
  - /styles/：全局样式设置
  - /components/：组件样式如头像、社交图标等

#### ✅ Step 4：绑定免费域名
- 推荐使用：Vercel 的免费子域名（例如：yourname.vercel.app）
- 或者用：
  - [Freenom](https://www.freenom.com/) 提供的免费域名（如 .tk、.ml）
  - 配合 Cloudflare 免费 CDN 加速与自定义解析
 
### 📚 三、建议学习路径（按需掌握即可）
| 学习内容           | 用途             | 推荐资源（建议收藏）                                     |
| -------------- | -------------- | ---------------------------------------------- |
| Markdown       | 写简历、笔记、文章      | [Markdown 教程](https://markdown.tw/)            |
| Notion API 基础  | 网页连接 Notion 数据 | 看 NotionNext 的 GitHub 文档                       |
| Git & GitHub   | 版本控制 + 托管代码    | 廖雪峰教程 / B 站教学                                  |
| HTML + CSS     | 理解网页结构与样式      | MDN 入门 / [CSS布局指南](https://flexboxfroggy.com/) |
| Tailwind CSS   | 控制网页样式         | [官方文档](https://tailwindcss.com/docs) + 示例项目    |
| Next.js（React） | 前端网站结构和路由系统    | [Next.js 中文网](https://nextjs.frontendx.cn/)    |

### 🎁 Bonus：实用资源推荐
| 类型   | 名称 / 链接                                                | 简介                  |
| ---- | ------------------------------------------------------ | ------------------- |
| 博客模板 | [NotionNext](https://github.com/tangly1024/NotionNext) | 高颜值 Notion 博客框架     |
| 图床   | [sm.ms](https://sm.ms/) / GitHub 图床                    | 存放你要展示的生活照片         |
| 免费域名 | [Freenom](https://freenom.com/)                        | 可申请 `.tk` 等免费域名     |
| 部署平台 | [Vercel](https://vercel.com/)                          | 免费部署，绑定 GitHub 自动上线 |



