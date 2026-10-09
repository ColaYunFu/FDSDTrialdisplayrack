# GitHub Pages 部署说明

本项目是纯静态网页，入口文件是仓库根目录的 `index.html`，不需要构建步骤。

## 发布前先确认账户计划

GitHub Pages 在 GitHub Free 个人账户下仅支持公开仓库；GitHub Pro、Team 和 Enterprise 计划可从私有仓库发布。请不要为了试用而自动更改仓库可见性。官方说明：
https://docs.github.com/en/pages/getting-started-with-github-pages/creating-a-github-pages-site

## 启用 Pages

1. 打开仓库 `ColaYunFu/Storage-room`。
2. 进入 **Settings → Pages**。
3. 在 **Build and deployment** 里，将 Source 选为 **Deploy from a branch**。
4. Branch 选择 `main`，目录选择 `/(root)`，点击 **Save**。
5. 等待发布完成后，在 Pages 页面点击 **Visit site**。项目网址通常形如 `https://colayunfu.github.io/Storage-room/`，以设置页给出的链接为准。

如果在 Settings → Pages 中无法从私有仓库发布，先停在这里，不需要更改仓库状态；可选择升级支持私有 Pages 的计划，或由仓库所有者自行决定是否公开仓库。

## 数据与隐私

工作台默认把任务、便签和每日目标保存在访问者当前浏览器的 `localStorage`，不会自动同步到其他设备。请定期使用页面里的 JSON 导出功能备份数据。

网页代码与浏览器里的任务数据是分开的；但公开发布后，网页本身可被所有人访问。不要把密码、访问令牌或其他敏感信息放入网页代码或仓库。

## 本地预览

直接用现代浏览器打开 `index.html`，或在项目目录运行：

```bash
python -m http.server 8080
```

然后访问 `http://localhost:8080`。