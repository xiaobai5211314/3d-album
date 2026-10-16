# 3D 水晶球手势交互相册 (3d.21212121.xyz)

[![Deploy](https://github.com/xiaobai5211314/3d-album/actions/workflows/deploy.yml/badge.svg)](https://github.com/xiaobai5211314/3d-album/actions/workflows/deploy.yml)
[![Website](https://img.shields.io/badge/online-3d.21212121.xyz-blue)](https://3d.21212121.xyz)

> 基于 Three.js 与 MediaPipe 打造的 3D 照片墙与水晶球空间，支持摄像头 AI 手势隔空操作（平掌旋转、捏合缩放、握拳爆发、挥手切形、剪刀手流星）与多端无缝触控/鼠标浏览。

---

## 🌐 访问地址
- 官方独立域名：[https://3d.21212121.xyz](https://3d.21212121.xyz)
- 生产服务器根目录：`/www/wwwroot/3d.21212121.xyz/`

## 🖐️ 手势控制系统 (MediaPipe HandLandmarker)
| 手势 | 触发动作 | 交互效果 |
| :--- | :--- | :--- |
| 🖐 **平掌平移** | 空间旋转 (Rotate) | 张开手掌在镜头前移动，3D 照片球随手势 360° 自适应平滑旋转 |
| 🤏 **双指捏合** | 景深缩放 (Zoom) | 拇指与食指捏合距离驱动相机 Z 轴景深，自由推拉微距视角 |
| ✊ **握拳聚拢** | 能量爆发 (Burst) | 握紧拳头锁定视角聚拢能量，松开时触发星空粒子流星爆发特效 |
| 👋 **快速挥手** | 形态切换 (Swipe) | 手掌快速向左/向右划过，流畅循环切换 4 种三维空间几何形态 |
| ✌️ **剪刀手** | 流星雨 (Meteors) | 比出胜利 V 字手势，召唤划破天际的彩虹星芒与深空流星雨 |
| 👌 **OK手势** | 自动巡航 (Auto Orbit) | 拇指食指相扣成圆，开启/暂停 3D 水晶球宇宙漫游自动巡航 |

## 🛠️ 技术栈与特性
- **渲染核心**：Three.js 0.160.0 / CSS3DRenderer / TrackballControls / WebGL (3200+ 动态星空粒子)
- **手势引擎**：MediaPipe Tasks-Vision 0.10.3 (21 关节点骨骼雷达画中画 PIP 可视化)
- **空间音效**：Web Audio API 原生合成晶体和弦与交互声效（0 额外音频请求，零延迟）
- **高速 CDN**：Three.js、MediaPipe 视觉模型与 71 张精选照片全量托管于又拍云 CDN `https://guzhicdn.21212121.xyz/`
- **站群互联**：右上角集成统一高质感半透明玻璃态品牌胶囊导航（`xb-brand-pill-container`），直达博客主站（`https://21212121.xyz`）与全景导航站（`https://nav.21212121.xyz`）。

## 🚀 自动部署与 CI/CD
本项目已配置 GitHub Actions 自动化持续集成：
- 当向 `main` 分支提交（Push）或合并代码时，GitHub Actions 会自动通过安全 SSH 密钥同步最新代码至生产服务器 `/www/wwwroot/3d.21212121.xyz`。

## 📄 授权与许可
详细规范请参考 [AGENTS.md](./AGENTS.md)。
Personal Open Source Project · All Rights Reserved.
