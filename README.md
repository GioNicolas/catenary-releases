<div align="center">

# Catenary

### The Infinite Spatial Canvas IDE for AI Coding Agents

An infinite 2D zoomable workspace designed for coordinating multi-agent workflows.  
Wire agents together with visual cables, isolate work into parallel task islands, and code 100% local-first.

[![Release](https://img.shields.io/github/v/release/GioNicolas/catenary-releases?style=for-the-badge&color=blue)](https://github.com/GioNicolas/catenary-releases/releases/latest)
[![Downloads](https://img.shields.io/github/downloads/GioNicolas/catenary-releases/total?style=for-the-badge&color=success)](https://github.com/GioNicolas/catenary-releases/releases)
[![Platform](https://img.shields.io/badge/Platform-macOS%20%7C%20Windows%20%7C%20Linux-orange?style=for-the-badge)](https://thecatenary.app)
[![Local First](https://img.shields.io/badge/Architecture-100%25%20Local--First-purple?style=for-the-badge)](https://thecatenary.app)

[**Website & Download**](https://thecatenary.app) · [**Report Issue**](https://github.com/GioNicolas/catenary-releases/issues) · [**Changelog**](https://github.com/GioNicolas/catenary-releases/releases)

</div>

---

## 🚀 Quick Install

### macOS (Homebrew)
```bash
brew tap gionicolas/catenary
brew install --cask catenary
```

### Windows (Winget)
```powershell
winget install Catenary.Catenary
```

### Direct Downloads (Latest v1.0.5)

| Operating System | Package Format | Download Link |
| :--- | :--- | :--- |
| **macOS (Apple Silicon)** | `.dmg` / `.zip` | [Download arm64.dmg](https://github.com/GioNicolas/catenary-releases/releases/latest/download/Catenary-1.0.5-arm64.dmg) |
| **macOS (Intel)** | `.dmg` / `.zip` | [Download x64.dmg](https://github.com/GioNicolas/catenary-releases/releases/latest/download/Catenary-1.0.5-x64.dmg) |
| **Windows (x64)** | Setup `.exe` / `.zip` | [Download Setup.exe](https://github.com/GioNicolas/catenary-releases/releases/latest/download/Catenary-Setup-1.0.5.exe) |
| **Linux (Universal)** | `.AppImage` | [Download AppImage](https://github.com/GioNicolas/catenary-releases/releases/latest/download/Catenary-1.0.5.AppImage) |
| **Linux (Debian/Ubuntu)** | `.deb` | [Download .deb](https://github.com/GioNicolas/catenary-releases/releases/latest/download/catenary_1.0.5_amd64.deb) |

---

## ✨ Key Features

- 🔌 **Visual Context Wires:** Connect agent terminals together with visual cables. Pipe output buffers from planning models directly into execution agents seamlessly.
- 🏝️ **Task Islands & Maestro Mode:** Spin up isolated workspace islands on the 2D canvas with dedicated Git Worktrees. Run full agent squads (Architect, Implementer, QA Tester, Reviewer) in parallel without branch collision.
- ⚡ **Native GPU-Accelerated Terminals:** Backed by native C++ `node-pty` and `@xterm/xterm` with WebGL rendering, maintaining steady 60 FPS even under heavy build logs.
- 🔒 **100% Local-First & Private:** No cloud accounts, zero telemetry, full offline capability. Your code, worktrees, and API keys remain strictly on your machine.
- 🖥️ **Unified Spatial Workspace:** Monaco code editors, PTY terminals, local embedded webview browser, and documentation readers arranged side-by-side on an infinite zoomable canvas.

---

## 🛠️ Tech Stack & Under the Hood

- **Desktop Shell:** Electron 41 + Node.js (Strict Context Isolation)
- **Frontend & Canvas:** React 18, TypeScript, Tailwind CSS, SVG Bézier Curves
- **Editor Engine:** Monaco Editor (VS Code core)
- **Terminal Engine:** node-pty (C++ native PTY) + xterm.js with WebGL GPU addon
- **State & Persistence:** Zustand + Atomic JSON persistence (`.cate/workspace.json`)

---

## 🐞 Bug Reports & Feature Requests

Found a bug or have an idea to make Catenary better?  
Please [open an issue here](https://github.com/GioNicolas/catenary-releases/issues) on GitHub or send a e-mail to: support@thecatenary.app .

---

<div align="center">
  <sub>Engineered by Giorgio Nícolas · Distributed globally · <a href="https://thecatenary.app">thecatenary.app</a></sub>
</div>
