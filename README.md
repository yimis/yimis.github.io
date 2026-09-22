# 🌱 种子发芽占位页

> 这里呀，本来要长出一个网站的。
> 可惜站长忘了给它浇水，这颗网站小种子被随手塞进了仓库角落……
> 等哪天他突然想起它，就搬出来晒太阳、正式上线！

一个**单文件**的「网站施工中」占位页模板，fork 之后改三处就能变成你自己的：

1. 页面里的文案和署名
2. 邮箱地址（记得保持打码写法，见下文）
3. 仓库名 / 域名

## 特点

- 只有一个 `index.html`，零依赖、零构建、零框架
- 白色 + 绿色的清新风格，移动端自适应
- 邮箱以打码形式展示（如 `xxx#example.com`，标注「把 `#` 换成 `@`」），点击时才由脚本拼出真实链接，复制源码时请把邮箱一并替换

## 部署到 GitHub Pages

1. Fork 或新建仓库，把 `index.html` 放在**仓库根目录**
2. `Settings → Pages → Source` 选择 `Deploy from a branch`，分支 `main` + 根目录
3. 完事。推送即可访问 `https://<你的用户名>.github.io/<仓库名>/`
   （若仓库名为 `<你的用户名>.github.io`，则直接是 `https://<你的用户名>.github.io/`）

## 绑定自定义域名（可选）

1. 仓库根目录添加 `CNAME` 文件，内容一行：`<你的域名.com>`
2. `Settings → Pages → Custom domain` 填入同一个域名
3. DNS 侧：
   - 根域名：`A` 记录指向 Pages 的 IP（启用 Enforce HTTPS 后可开 `404 page → GitHub Pages`）
   - `www`：`CNAME` 指向 `<你的用户名>.github.io`
