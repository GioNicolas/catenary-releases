<div align="center">

# Catenary

### The Infinite Spatial Canvas IDE for AI Coding Agents

[![Release](https://img.shields.io/github/v/release/GioNicolas/catenary-releases?style=for-the-badge&color=blue)](https://github.com/GioNicolas/catenary-releases/releases/latest)
[![Downloads](https://img.shields.io/github/downloads/GioNicolas/catenary-releases/total?style=for-the-badge&color=success)](https://github.com/GioNicolas/catenary-releases/releases)
[![Platform](https://img.shields.io/badge/Platform-macOS%20%7C%20Windows%20%7C%20Linux-orange?style=for-the-badge)](https://thecatenary.app)
[![Local First](https://img.shields.io/badge/Architecture-100%25%20Local--First-purple?style=for-the-badge)](https://thecatenary.app)

[**Website & Download**](https://thecatenary.app) · [**Report Issue**](https://github.com/GioNicolas/catenary-releases/issues) · [**Changelog**](https://github.com/GioNicolas/catenary-releases/releases)

</div>

---

Draw a line from one agent to another and their work connects. What one finishes becomes what the next one starts — flowing on its own, or only when an agent asks for it. You decide, wire by wire. No more copying context between windows.

It's a full workspace, not a chat box. Terminals, Monaco editors, browsers, documents and parallel git worktrees all live on the same surface — pan, zoom, drag anything anywhere. Close the folder and everything comes back exactly where you left it.

Then turn on **Maestro Mode**, and one agent builds its own team: it recruits up to five agents, hands each one the objective, and wires them to itself. Every move it makes stops at a card you can edit before you approve it. The team organizes itself. You stay the one who says yes.

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

## ✨ What's Inside

- **Wires between agents** — a directed line from one terminal to another. Set it to relay automatically when the source goes quiet, or leave it as a standing permission so the agent downstream only receives what it asks for.
- **Maestro Mode** — one agent recruits, briefs and connects a team of up to five. Off by default, flipped by a human click, and every action it takes opens an editable approval card before anything appears on the canvas.
- **Agent-aware terminals** — supported agent CLIs (Claude Code, Codex, Cursor, Grok, OpenCode, Pi) report turn start, turn end and permission prompts, so each panel shows whether its agent is working, waiting or done — and notifies you the moment one needs an answer.
- **Worktrees for parallel branches** — describe what you're working on and Catenary creates the worktree and branch. Each gets a colour that follows it through the sidebar, the dock tabs and its own territory on the canvas.
- **Infinite canvas + docking** — float panels anywhere, dock them as tabs and splits, or detach them into their own windows. The whole layout is restored when you reopen the folder.
- **A full IDE around it** — Monaco editors with diffs, embedded browsers, document viewers, a git-aware file tree, project search, source control and a built-in agent chat.
- **Local and remote take the same path** — one runtime daemon serves every workspace. Point Catenary at a host over SSH or WSL and terminals, git, search and agents run there while editors, browsers and the canvas stay local.
- **A CLI agents can call** — from inside a terminal, `catenary` drives a browser panel, reads another terminal, opens files and manages panels. Settings → CLI grants each surface separately for reading and for controlling.
- **100% Local-First & Private** — no cloud accounts, zero telemetry, full offline capability. Your code, worktrees, and API keys remain strictly on your machine.

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
Please [open an issue here](https://github.com/GioNicolas/catenary-releases/issues) on GitHub or send an email to: [support@thecatenary.app](mailto:support@thecatenary.app).

---

<div align="center">
  <sub>Engineered by Giorgio Nícolas · Distributed globally · <a href="https://thecatenary.app">thecatenary.app</a></sub>
</div>
