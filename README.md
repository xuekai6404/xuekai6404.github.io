# EtaNotes Website

这是 EtaNotes 的 GitHub Pages 网站，包含产品介绍页面和 app-ads.txt 文件。

## 文件说明

- `index.html` - 产品介绍主页
- `app-ads.txt` - 广告验证文件（用于 Google AdMob）
- `assets/style.css` - 网站样式文件

## 部署说明

### GitHub Pages 设置

1. 在 GitHub 仓库中，进入 **Settings** > **Pages**
2. 在 **Source** 部分，选择：
   - Branch: `main` (或 `master`)
   - Folder: `/docs/website`
3. 点击 **Save** 保存设置
4. 网站将在几分钟内部署到：`https://[username].github.io/EtaNotes/`

### app-ads.txt 配置

1. 打开 `app-ads.txt` 文件
2. 将 `pub-XXXXXXXXXXXXXXXX` 替换为您的实际 Google AdMob 发布商 ID
3. 发布商 ID 可以在 [Google AdMob 控制台](https://apps.admob.com/) 的 **设置** > **账户信息** 中找到
4. 提交更改后，文件将自动部署

### 验证 app-ads.txt

部署后，可以通过以下方式验证：

1. 访问：`https://[username].github.io/EtaNotes/app-ads.txt`
2. 确认文件可以正常访问且内容正确
3. 在 Google AdMob 中验证域名所有权（如需要）

## 更新下载链接

在 `index.html` 中更新实际的 App Store 和 Google Play 下载链接：

- iOS 下载链接：找到 `id="ios-download"` 的 `<a>` 标签，更新 `href` 属性
- Android 下载链接：找到 `id="android-download"` 的 `<a>` 标签，更新 `href` 属性

## 注意事项

- app-ads.txt 文件更新后，可能需要几小时才能被广告网络抓取
- 确保使用 HTTPS 访问（GitHub Pages 自动提供）
- 如需使用自定义域名，需要在 GitHub Pages 设置中配置
