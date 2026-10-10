# 张林 Lydia · 个人说明书网站

这是当前网站的完整静态版本，包含首页、商品审核案例详情页、照片及简历下载。无需安装依赖、无需构建、无需 API 密钥。

## 上传到 GitHub

1. 解压本压缩包。不要直接把 ZIP 文件上传到仓库。
2. 打开目标仓库，选择 Add file → Upload files。
3. 上传解压后全部文件及 assets 文件夹，点击 Commit changes。
4. 确认仓库根目录直接有 index.html、case-audit.html、assets/、README.md 和 .nojekyll。不要多套一层文件夹。

如果浏览器未上传隐藏的 .nojekyll，可在仓库 Add file → Create new file 中创建名为 .nojekyll 的空文件。本网站没有需要特殊处理的目录，遗漏它通常不影响页面展示。

## 开启 GitHub Pages

进入仓库 Settings → Pages：
- Source 选择 Deploy from a branch。
- Branch 选择实际上传文件所在分支（通常为 main）。
- 目录选择 / (root)，点击 Save。

等待发布完成，在 Pages 页面打开 GitHub 给出的 Visit site 链接。以 GitHub 显示的地址为准。

本项目全部使用相对路径，支持用户主页仓库和普通项目仓库。无需填写 Build command，也不需要 GitHub Actions 工作流。

## 文件与功能

- index.html：首页（包含样式与脚本）
- case-audit.html：代表案例详情页
- assets/：页面所需的照片和 zhanglin-resume.pdf
- .nojekyll：静态发布标记

当前效果包含：小照片拼贴、点击放大、实习章节展开、邮件入口、简历下载、麦金色圆点与金黄散雾光晕。鼠标特效在触屏或减少动态效果设置下关闭。

简历下载使用本次提供的“南开大学-张林-金融专业-AI岗位(2).pdf”原文件。网页不显示实习时间，PDF 文件内容保留原样。

## 本地查看与更新

可直接双击 index.html 预览；复制邮箱功能建议在 HTTPS 发布后使用。
更新时替换对应 HTML 或 assets 文件即可。替换简历请保持 assets/zhanglin-resume.pdf 文件名。

## 发布说明

该包不包含原托管平台的登录限制。启用公开 GitHub Pages 后，网页照片、邮箱和下载简历可被访问者查看与下载。

## 常见问题

- 显示 README 而非网页：检查 index.html 是否直接放在所选发布目录。
- 图片不显示：确认 assets 文件夹完整，文件名大小写一致。
- 更新后仍是旧版：等待 Pages 部署完成，再强制刷新页面。
- 不要把整个文件夹作为新的一层上传；应上传文件夹里面的内容。
