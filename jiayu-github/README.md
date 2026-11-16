# JIAYU 个人作品集

## GitHub Pages 部署
1. 将本目录内的全部文件上传到 GitHub 仓库根目录。
2. 在 Settings → Pages 中选择 Deploy from a branch，分支 main，目录 / (root)。
3. 保存后等待 GitHub Pages 部署完成。

## 文件结构
- index.html：页面结构
- css/style.css：全部样式
- js/main.js：页面互动、项目浏览与动效
- js/lanyard.js：3D 吊牌与后续交互
- assets/images：去重后的图片，包括项目长图与二维码
- assets/fonts：内嵌字体提取文件
- assets/svg：页面 SVG 独立副本

SVG 在 HTML 内仍保留交互必需的内联版本，以维持擦除动画、路径查询和样式继承；独立 SVG 副本可单独编辑使用。

请通过 HTTP 服务器预览，避免直接双击 HTML 导致 ES module 加载受限。可运行 npx serve . 。

GSAP、Lenis、Matter.js 与 Three.js 从 CDN 加载，需要联网。照片、项目图、二维码和字体均为本地资源。两张项目长图转为质量 88 的 JPEG，保持原始像素尺寸；其他图片保持原样。

页面包含公开联系方式和微信二维码，发布后访问者可以查看。
