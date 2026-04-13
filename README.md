# Tunnel Solver: Rapid Mechanical Assessment of Deep Tunnels

[![Version](https://img.shields.io/badge/version-v0.11--beta-blue)](https://github.com/YOUR_USERNAME/Tunnel-Solver/releases)
[![Platform](https://img.shields.io/badge/platform-Windows-0078d7)](https://github.com/YOUR_USERNAME/Tunnel-Solver/releases)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

**Tunnel Solver** is a high-performance Windows application designed for the rapid assessment of elasto-plastic deformation in deeply-buried tunnels. It strictly couples the **Non-linear Analytical Rock (NAR)** constitutive model with a semi-analytical **Boundary Value Problem (BVP)** solver.

Developed by a collaborative research team from **Monash University**, **The University of Sydney**, and **Wuhan University**.

---

## 🚀 Download & Installation

This software is distributed as a standalone Windows executable. **No Python environment or installation is required.**

1.  Navigate to the **[Releases](https://github.com/YOUR_USERNAME/Tunnel-Solver/releases)** page.
2.  Download the latest package: `Tunnel_Solver_v0.11.zip`.
3.  Extract the ZIP file to a local folder.
4.  Double-click `Tunnel_Solver.exe` to launch the application.

*Note: Some antivirus software may flag the EXE as an unknown program. Please select "Run anyway" or run as administrator.*

---

## ✨ Key Features

* **Integrated Graphical Interface:** Multi-page GUI optimized for high-DPI (1080p/4K) displays, supporting real-time data interaction.
* **Adaptive LM Inversion Engine:** Employs a robust, unconstrained Levenberg-Marquardt (LM) algorithm to identify NAR parameters from triaxial data without artificial truncation.
* **NAR Constitutive Model:** Captures the full stress-strain process, including pre-peak hardening, post-peak softening, and complex lateral dilatancy.
* **Empirical Mapping Module:** Seamlessly translates macroscopic descriptors ($GSI$, $\sigma_{ci}$, $m_i$, $D$) and strain-rate effects into intrinsic constitutive parameters.
* **Semi-Analytical BVP Solver:** Executes millisecond-level recursive discretization for hydrostatic tunnel responses, bypassing the "black-box" nature of traditional numerical codes.

---

## 📸 Screenshots

| 1. Triaxial Calibration | 2. Empirical Mapping | 3. Tunnel Simulation |
| :---: | :---: | :---: |
| ![Calibration](Gui_Figues/Calibration_lab_tests.png) | ![Empirical](Gui_Figues/empirical_method.png) | ![Simulation](Gui_Figues/deep_tunnel.png) |

*(Recommended: Create a `docs/images` folder in your repo and upload your screenshots there to replace these placeholders.)*



---

## 📜 Citation

If you use this software in your research, please cite our corresponding work:

```bibtex
@article{li2026rapid,
  title={Rapid assessment of the mechanical response of deeply-buried tunnels: Governing equations, parameter calibration, and GUI design},
  author={Li, Zhihang and Zhang, Chunshun and Shen, Luming and Tang, Yaolan and Zhao, Jian},
  journal={Preprint},
  year={2026}
}
