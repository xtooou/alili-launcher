<div align="center">

# 🚀 Alili Launcher (阿里里启动器)
### 专为 ComfyUI 打造的现代化、专业、极简生态管理平台

[![Platform](https://img.shields.io/badge/Platform-Windows%2010%2F11%20(64--bit)-0078D6?style=flat-square&logo=windows)](https://github.com)
[![Electron](https://img.shields.io/badge/Electron-Desktop-47848F?style=flat-square&logo=electron)](https://www.electronjs.org/)
[![ComfyUI](https://img.shields.io/badge/ComfyUI-Portable%20Compatible-blueviolet?style=flat-square)](https://github.com/comfyanonymous/ComfyUI)
[![License](https://img.shields.io/badge/License-Free%20for%20All-brightgreen?style=flat-square)]()

**告别简陋黑框报错与磁盘爆炸，重构你的 ComfyUI 创作体验。**

[💻 桌面版下载](#-桌面版下载) • [📺 基础功能教程](#-基础功能教程) • [✨ 功能亮点](#-功能亮点) • [❓ 常见问题](#-常见问题)

---

</div>

## 📖 项目简介

**Alili 启动器** 让你告别简陋的黑框报错与"磁盘爆炸"式手动部署，用一套图形化管理面板重构 ComfyUI 的创作体验。智能识别根目录、一键启动内核、实时设备体检、内置便携 Git——把专业门槛降到最低，让创作回归创作本身。

---

## ✨ 功能亮点

### 🔍 智能识别 · 零配置
- 自动识别 ComfyUI 根目录与 `python.exe`，完美兼容官方**便携版**目录结构（`ComfyUI` + 同级 `python_embeded`）。
- 不论选中外层整合包还是内层 `ComfyUI` 文件夹，都能精准定位。

### 🚀 一键启动内核
- `cpu` / `fp16` 双开关，自定义启动参数追加，用户的参数优先级最高。
- 自动注入 UTF-8 环境变量，彻底解决中文 Windows 下 GBK 乱码问题。

### 🩺 设备体检
- 实时读取 **Python / Pytorch 版本、GPU 型号与显存占用、Git 版本**，环境状态一目了然。
- 自动识别内置 MinGit，标注"便携 Git"状态。

### 🧰 内置便携 Git（MinGit）
- 随包集成免安装 Git，让 **ComfyUI-Manager** 直接识别，插件安装不再卡在 Git 环节。

### 💻 系统托盘常驻
- 关闭窗口自动最小化到托盘，后台常驻不占任务栏，需要时一点即回。

### 📦 本地便携 · 自研更新
- 数据与缓存目录重定向到程序同级，U 盘随身带、即插即用。
- 自研增量更新器 + 国内高速镜像源，更新过程不卡死。

### 🌐 多形态分发
- 同时提供 **NSIS 安装版 / 便携版（standalone）/ ZIP** 三种形态，自由选择。

---

## 📸 界面预览

<!-- 截图请放置于 docs/ 目录后替换下方路径 -->
| 主控制台 | 设备体检 |
| :---: | :---: |
| ![主控制台](docs/preview-main.png) | ![设备体检](docs/preview-device.png) |
| 一键启动 ComfyUI | Python / GPU / Git 状态 |

| 启动日志 | 系统托盘 |
| :---: | :---: |
| ![启动日志](docs/preview-log.png) | ![托盘](docs/preview-tray.png) |
| 实时内核日志 | 最小化到托盘 |

> 💡 截图占位：请将实际软件截图放入 `docs/` 目录，并替换上方文件名即可自动生效。

---

## 📺 基础功能教程

> 完整视频教程正在筹备中，可先关注作者 B 站主页获取最新动态：
>
> 👉 **B 站教程空间**：https://space.bilibili.com/67359822
>
> （具体教学视频上线后，此处会补充对应分集链接。）

**图文速览：**
1. 打开启动器，点击「选择 ComfyUI 根目录」，选中整合包文件夹。
2. 在主面板确认识别出的 `python.exe` 路径无误。
3. 按需开启 `cpu` / `fp16` 开关，点击「启动 ComfyUI」。
4. 查看实时启动日志与设备体检信息，浏览器自动打开 ComfyUI 界面。

---

## ❓ 常见问题

**Q：支持哪些 ComfyUI 版本？**
> 兼容官方**便携版**目录结构（根目录下 `ComfyUI` 与同级 `python_embeded`）。手动部署版只要能找到 `main.py` 与 `python.exe` 也可识别。

**Q：我需要自己安装 Python 吗？**
> 便携版已自带内嵌 Python，无需额外安装；若使用系统全局 Python，可在设置中手动指定 `python.exe`。

**Q：启动失败 / 一闪而过？**
> 依次检查：① `python.exe` 路径是否正确；② 显卡 CUDA 驱动是否就绪；③ 默认端口（8188）是否被占用；④ 查看启动日志的具体报错。

**Q：插件安装时提示找不到 Git？**
> 启动器已内置 MinGit 并自动注入环境变量，正常情况下 ComfyUI-Manager 可直接使用；若仍报错，请确认未被安全软件拦截。

**Q：支持 macOS / Linux 吗？**
> 当前版本为 Windows 专属，macOS / Linux 版本正在规划中。

---

## 📥 桌面版下载

| 平台 | 下载 |
| :--- | :--- |
| 🪟 Windows | [Windows 下载](#) （请替换为你的发布页地址） |
| 🍎 macOS | 暂未提供 |

> 提供 NSIS 安装版（支持自定义安装目录）、便携版与 ZIP 三种形态，安装完成后默认自动启动。

---

## 📄 开源协议

本项目**免费向所有人开放**使用。作者：**阿里里**。

⭐ 如果这个项目帮到了你，欢迎 Star 与分享！
