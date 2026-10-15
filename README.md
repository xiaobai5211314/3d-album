# 3D 水晶球手势交互相册 (3d.21212121.xyz)

[![Deploy](https://github.com/xiaobai5211314/3d-album/actions/workflows/deploy.yml/badge.svg)](https://github.com/xiaobai5211314/3d-album/actions/workflows/deploy.yml)
[![Website](https://img.shields.io/badge/online-3d.21212121.xyz-blue)](https://3d.21212121.xyz)

> 基于 Three.js 打造的 3D 照片墙与元素周期表粒子展示，支持摄像头手势识别交互与三维滚轮缩放浏览。

---

## 🌐 访问地址
- 官方独立域名：[https://3d.21212121.xyz](https://3d.21212121.xyz)
- 生产服务器根目录：`/www/wwwroot/3d.21212121.xyz/`

## 🛠️ 技术栈与特性
- **渲染核心**：Three.js 0.160.0 / CSS3DRenderer / TrackballControls / WebGL
- **手势引擎**：MediaPipe Tasks-Vision (HandLandmarker)
- **CDN 加速**：Three.js 模块、Tween.js 及 MediaPipe 视觉模型资产全量托管于 `https://guzhicdn.21212121.xyz/`，大幅减少源站带宽负荷。
- **站群互联**：界面右上角集成高质感品牌胶囊导航（`xb-brand-pill-container`），直达岁月静好博客主站（`https://21212121.xyz`）与全景导航站（`https://nav.21212121.xyz`）。

## 🚀 自动部署与 CI/CD
本项目已配置 GitHub Actions 自动化持续集成：
- 当向 `main` 分支提交（Push）或合并代码时，GitHub Actions 会自动通过安全 SSH 密钥同步最新代码至生产服务器 `/www/wwwroot/3d.21212121.xyz`。

## 📄 授权与许可
详细规范请参考 [AGENTS.md](./AGENTS.md)。
Personal Open Source Project · All Rights Reserved.
