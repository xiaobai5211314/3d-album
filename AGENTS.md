# 3D相册 项目规范与架构 (AGENTS.md)

## 1. 项目定位与服务信息
- **项目名称**：3D 水晶球手势交互相册
- **独立二级域名**：`https://3d.21212121.xyz`
- **技术栈**：Three.js / MediaPipe Hands / WebGL / CSS3 3D
- **静态资源 CDN**：Three.js 0.160.0、Tween.js、MediaPipe Tasks-Vision 与 HandLandmarker 模型全量托管于高速静态 CDN `https://guzhicdn.21212121.xyz/`，源站 0 静态大文件负担。
- **生产服务器根目录**：`/www/wwwroot/3d.21212121.xyz/`
- **自动化部署**：通过 GitHub Actions 联动，代码提交至 `main` 分支后自动同步至生产环境。

## 2. 核心架构与功能说明
基于 Three.js 打造的 3D 照片墙与元素周期表粒子展示，支持摄像头手势识别交互与三维滚轮缩放浏览。
右上角集成统一高质感半透明玻璃态品牌胶囊导航（`xb-brand-pill-container`），提供指向个人主博客（`https://21212121.xyz`）与站群全景导航（`https://a.21212121.xyz`）的无缝直达能力。

## 3. 规范与维护约定
- **单一规则源**：遵循本 `AGENTS.md`，严禁新增冗余规则文件。
- **自适应要求**：必须保持移动端（竖屏/横屏）与桌面端良好排版，触控目标不小于 44px。
- **整洁契约**：禁止提交备份脚本（*.bak、*.old），提交前确保本地与线上代码同步。

## 4. 相关文档
- [README.md](./README.md)
