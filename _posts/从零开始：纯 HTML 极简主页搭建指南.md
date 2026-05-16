## 从零开始：纯 HTML 极简主页搭建指南

**不需要 Jekyll，不需要后端**，只需一个 `index.html` 文件和 GitHub Pages，十分钟搭建属于你的高逼格个人主页。

---

## 为什么选择纯 HTML 极简主页

- **零依赖**：无框架、无打包工具、无数据库。
- **极致轻量**：页面体积通常小于 50KB，加载飞快。
- **高逼格**：极简设计本身就是一种审美声明。
- **完全可控**：每一行代码都属于你自己。
- **永久免费**：GitHub Pages 提供无限流量和 HTTPS。

---

## 准备工作

1. 一个 **GitHub** 账号（如果没有，去 [github.com][1] 注册，免费）。
2. 本地任意一个**文本编辑器**（VS Code、Sublime、记事本都可以）。
3. 愿意动手的心态。

[1]: https://github.com

---

## 第一步：创建你的第一个 index.html

在你的电脑上新建一个文件夹，比如 `my-homepage`，在里面创建一个文件 `index.html`，用编辑器打开。

复制下面的 **极简模版**：

```html
<!DOCTYPE html>
<html lang="zh-CN">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>你的名字 · 极简主页</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        body {
            background: #faf9f8;
            font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Helvetica, Arial, sans-serif;
            line-height: 1.6;
            color: #1e1e2a;
            padding: 2rem;
            min-height: 100vh;
            display: flex;
            align-items: center;
            justify-content: center;
        }
        .container {
            max-width: 680px;
            width: 100%;
            margin: 0 auto;
        }
        h1 {
            font-size: 2.8rem;
            font-weight: 600;
            letter-spacing: -0.02em;
            margin-bottom: 0.5rem;
            border-left: 5px solid #0366d6;
            padding-left: 1.2rem;
        }
        .sub {
            font-size: 1.2rem;
            color: #4a4a5a;
            margin-bottom: 2rem;
            padding-left: 1.7rem;
        }
        .bio {
            background: white;
            padding: 2rem;
            border-radius: 24px;
            box-shadow: 0 8px 20px rgba(0,0,0,0.02), 0 2px 6px rgba(0,0,0,0.05);
            margin: 1.5rem 0;
        }
        p {
            margin-bottom: 1rem;
        }
        .links {
            display: flex;
            flex-wrap: wrap;
            gap: 1rem;
            margin-top: 2rem;
            padding-left: 1.7rem;
        }
        .links a {
            text-decoration: none;
            color: #0366d6;
            font-weight: 500;
            border-bottom: 1px solid transparent;
            transition: 0.2s;
        }
        .links a:hover {
            border-bottom-color: #0366d6;
        }
        hr {
            margin: 2rem 0;
            border: none;
            height: 1px;
            background: #e2e2e6;
        }
        footer {
            text-align: center;
            font-size: 0.85rem;
            color: #888;
            margin-top: 3rem;
        }
        @media (max-width: 500px) {
            body { padding: 1.2rem; }
            h1 { font-size: 2rem; }
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>你好，我是 <span id="name">林轻扬</span></h1>
        <div class="sub">写代码 · 读诗 · 构建安静的数字角落</div>

        <div class="bio">
            <p>🎯 全栈开发者，热爱 <strong>极简设计</strong> 与 <strong>可读性优先</strong> 的代码。</p>
            <p>📖 当前正在探索：Web 性能、静态站点、数字花园。</p>
            <p>☕ 相信一句老话：<em>“完美不是无以复加，而是无可删减。”</em></p>
        </div>

        <div class="links">
            <a href="#">🐙 GitHub</a>
            <a href="#">📧 邮件</a>
            <a href="#">📝 笔记/博客</a>
            <a href="#">🐦 X / 微博</a>
        </div>

        <hr />

        <footer>
            © 2026 xxx · 用 HTML 与耐心搭建
        </footer>
    </div>
</body>
</html>