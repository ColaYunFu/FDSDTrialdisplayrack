# GitHub Pages 部署说明

本项目是静态网页，入口文件为仓库根目录的 `index.html`，无需构建步骤。

## 发布前先确认账户计划

GitHub Pages 在 GitHub Free 个人账户下仅支持公开仓库；GitHub Pro、Team 和 Enterprise 计划可从私有仓库发布。请勿为了试用而自动更改仓库可见性。官方说明：https://docs.github.com/en/pages/getting-started-with-github-pages/creating-a-github-pages-site

## 启用 Pages

1. 打开仓库 `ColaYunFu/Storage-room`。
2. 进入 **Settings → Pages**。
3. 在 **Build and deployment** 里，将 Source 选为 **Deploy from a branch**。
4. Branch 选择 `main`，目录选择 `/(root)`，点击 **Save**。
5. 等待发布完成后，在 Pages 页面点击 **Visit site**。通常项目网址形如 `https://colayunfu.github.io/Storage-room/`，以设置页给出的链接为准。

## 数据与隐私

工作台默认把任务和便签保存在访问者浏览器的 `localStorage`，不会自动同步到其他设备。定期使用页面内的 JSON 导出功能备份。发布为公开网站后，任何人都可以访问网页；不要在里面输入密码或其他敏感信息。

## 本地预览

直接用现代浏览器打开 `index.html`。
