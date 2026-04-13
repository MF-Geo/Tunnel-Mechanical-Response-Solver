# Tunnel Solver: Rapid Mechanical Assessment of Deep Tunnels

[![Version](https://img.shields.io/badge/version-v0.11--beta-blue)](https://github.com/你的用户名/Tunnel-Solver/releases)
[![Platform](https://img.shields.io/badge/platform-Windows-0078d7)](https://github.com/你的用户名/Tunnel-Solver/releases)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

**Tunnel Solver** 是一款专为深埋隧道围岩变形快速评估设计的 Windows 桌面应用程序。该软件将 **非线性分析岩石 (NAR)** 构型模型与半解析 **边值问题 (BVP)** 求解器深度结合，实现了从实验数据拟合到工程应用的一站式分析。

本项目由 **蒙纳士大学 (Monash University)**、**悉尼大学 (The University of Sydney)** 及 **武汉大学** 的科研团队联合开发。

---

## 🚀 下载与安装 (Download & Installation)

本软件以 Windows 独立可执行文件（EXE）形式发布，**无需安装 Python 环境。**

1. 前往 **[Releases](https://github.com/你的用户名/Tunnel-Solver/releases)** 页面。
2. 下载最新版本的压缩包：`Tunnel_Solver_v0.11.zip`。
3. 解压到本地文件夹。
4. 双击运行 `Tunnel_Solver.exe` 即可启动程序。

*注：部分杀毒软件可能会对未签名的 EXE 进行拦截，请点击“仍要运行”或以管理员权限运行。*

---

## ✨ 核心功能 (Key Features)

* **全功能桌面交互界面：** 基于 Python 深度定制的 GUI，支持 1080P/4K 高清屏自适应缩放。
* **自适应 LM 反演引擎：** 采用稳健的 Levenberg-Marquardt (LM) 算法，直接从三轴压缩实验数据中识别 NAR 模型参数。
* **NAR 构型模型：** 能够精确捕捉岩石从硬化到软化的连续强度演化以及复杂的侧向扩容特性。
* **经验映射系统：** 支持将地质强度指标 ($GSI$, $\sigma_{ci}$, $m_i$, $D$) 直接映射为 NAR 本构参数。
* **半解析 BVP 求解器：** 毫秒级完成静水压力下深埋隧道的应力-位移分布计算，效率远高于传统有限元数值模拟。

---

## 📸 软件截图 (Screenshots)

| 1. 三轴数据拟合 | 2. 经验参数映射 | 3. 隧道数值仿真 |
| :---: | :---: | :---: |
| ![拟合界面](docs/images/screenshot1.png) | ![映射界面](docs/images/screenshot2.png) | ![仿真界面](docs/images/screenshot3.png) |

*(建议：在仓库中新建 `docs/images` 文件夹并上传截图，替换上方链接)*

---

## 📖 理论背景 (Methodology)

软件核心算法基于 NAR (Non-linear Analytical Rock) 模型。不同于传统的线性或分段模型，NAR 模型使用统一的演化函数 $\xi(\gamma)$ 描述岩石全应力-应变过程，避免了数值计算中的奇点问题。

---

## 📜 论文引用 (Citation)

如果您在科研工作中使用了本工具，请引用我们的相关研究成果：

```bibtex
@article{li2026rapid,
  title={Rapid assessment of the mechanical response of deeply-buried tunnels: Governing equations, parameter calibration, and GUI design},
  author={Li, Zhihang and Zhang, Chunshun and Shen, Luming and Tang, Yaolan and Zhao, Jian},
  journal={Preprint},
  year={2026}
}
