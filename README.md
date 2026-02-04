# 守望先锋2 士兵76 自动压枪 罗技脚本（中文说明仓库）

> ⚠️ 本仓库仅提供 **中文说明与使用指引**，不包含源代码  
> 📦 源代码请前往主仓库查看与下载
<p align="center">
  <a href="https://github.com/panpenghui/logitech-lua-recoil" target="_blank">
    <img src="https://img.shields.io/badge/👉%20前往主仓库-点击跳转-blue?style=for-the-badge">
  </a>
</p>
📂 仓库结构说明

📘 本仓库：中文说明、使用指引

📦 主仓库：Lua 源代码与更新维护

👉 请始终以 主仓库代码 为准

📜 免责声明

本项目仅用于 学习 Lua 脚本与 Logitech G Hub 自动化功能。
请遵守你所使用游戏与平台的相关规则，风险自负。

⭐ 支持项目

如果这个项目对你有帮助：

给主仓库点个 ⭐

或分享给需要的朋友

感谢支持 🙏

<p align="center">
  <a href="https://github.com/panpenghui/logitech-lua-recoil">
    <img src="https://img.shields.io/badge/English%20Repo-Main-blue?style=for-the-badge">
  </a>
  <br><br>
  <a href="https://github.com/panpenghui/logitech-lua-recoil">
    <img src="https://img.shields.io/badge/源代码仓库-点击进入-green?style=for-the-badge">
  </a>
</p>

## 📌 项目简介

这是一个用于 **Logitech G Hub** 的 Lua 压枪脚本示例，  
通过模拟鼠标纵向移动，帮助提升连发时的稳定性。

本仓库作为 **中文说明入口**，方便中文用户理解脚本用途、配置方式与基本原理。

---
## 🎮 使用前提

- 罗技鼠标（支持 G Hub Lua）
- 已安装 **Logitech G Hub**
- 会在 G Hub 中添加并启用 Lua 脚本

---

## 🕹️ 功能说明

- 🔘 **中键**：开启 / 关闭压枪
- 🖱️ **左键**：射击时自动压枪
- 📉 **仅纵向控制**，不影响水平移动
- 🎯 支持前几发不压枪（更贴近实际手感）
- 🎲 轻微随机偏移，避免机械感

---

## ⚙️ 参数调整说明

脚本中可自行调整的核心参数：

```lua
shotInterval = 9      -- 射击间隔（ms）
verticalPull = 4     -- 压枪力度（数值越大越猛）
initialShots = 13    -- 前 N 发不压枪
---

常见调整建议

压不住 → 增大 verticalPull

压过头 → 减小 verticalPull

节奏不稳 → 微调 shotInterval
