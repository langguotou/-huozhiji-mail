# 霍志鸡邮箱

基于 mail.tm API 的临时邮箱静态站点。

## 部署方式

仓库已配置 GitHub Actions 工作流 `.github/workflows/deploy.yml`，推送到 `main` 分支后会自动部署到 GitHub Pages。

GitHub Pages 发布源需设置为 **GitHub Actions**（Settings → Pages → Build and deployment → Source）。

站点地址：https://langguotou.github.io/-huozhiji-mail/

## 本地文件说明

- `index.html` — 页面入口
- `css/style.css` — 样式
- `js/app.js` — mail.tm API 交互逻辑
- `docs/` — WebCatX / CatNative 桥接文档（原包附带）
- `appConfig.xlt` — 原 WebCatX 应用配置（原包附带）
- `assets/background.mp4` — 720p 压缩背景视频（约 1.8 MB）
- `.nojekyll` — 禁止 Jekyll 处理，保留原始文件
- `.github/workflows/deploy.yml` — GitHub Pages 部署工作流

原 zip 中的 `ze`（实际为 PNG）和 `appIcon.png` 未被网页引用，属于 WebCatX 打包资源，未包含在部署文件中。
