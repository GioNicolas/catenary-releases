<div align="center">

# Catenary

### The IDE for coding agents

Two lenses, one truth. Move between a code editor with local LSP, split terminals and a spatial canvas where your agents work in sync.

[![Release](https://img.shields.io/github/v/release/GioNicolas/catenary-releases?style=for-the-badge&color=blue)](https://github.com/GioNicolas/catenary-releases/releases/latest)
[![Downloads](https://img.shields.io/github/downloads/GioNicolas/catenary-releases/total?style=for-the-badge&color=success)](https://github.com/GioNicolas/catenary-releases/releases)
[![Platform](https://img.shields.io/badge/Platform-macOS%20%7C%20Windows%20%7C%20Linux-orange?style=for-the-badge)](https://thecatenary.app)
[![Local First](https://img.shields.io/badge/Architecture-100%25%20Local--First-purple?style=for-the-badge)](https://thecatenary.app)

[**Website**](https://thecatenary.app) · [**Docs**](https://thecatenary.app/docs) · [**Changelog**](https://thecatenary.app/changelog) · [**Report Issue**](https://github.com/GioNicolas/catenary-releases/issues)

</div>

---

Run Claude Code, Codex and Antigravity side by side, in one IDE built for them. The same work session has two lenses, and switching between them never restarts a process:

- **TerminalMap** — a focused grid of terminals, splits and tabs, with a cockpit of session cards that shows what every agent is doing and which one needs you.
- **Canvas** — an infinite surface where terminals, editors, browsers and worktrees float, and wires connect one agent's work to the next.

Around them, a real editor: Monaco with a shared local LSP for TypeScript and Python that your agents can query too, aware of what you have not saved yet.

---

## 🚀 Install

### macOS (Homebrew)
```bash
brew install --cask gionicolas/catenary/catenary
```

### Windows (PowerShell)
```powershell
irm https://thecatenary.app/install.ps1 | iex
```

### Linux (AppImage)
```bash
curl -sSL https://thecatenary.app/download/linux-appimage -o Catenary.AppImage
chmod +x Catenary.AppImage
```

### Direct downloads (always the latest version)

| Operating System | Package | Download |
| :--- | :--- | :--- |
| **macOS (Apple Silicon)** | `.dmg` | [Download](https://thecatenary.app/download/macArm64) |
| **macOS (Intel)** | `.dmg` | [Download](https://thecatenary.app/download/macIntel) |
| **Windows (x64)** | Setup `.exe` | [Download](https://thecatenary.app/download/windows) |
| **Linux (x64)** | `.AppImage` | [Download](https://thecatenary.app/download/linuxAppImage) |
| **Linux (Debian/Ubuntu)** | `.deb` | [Download](https://thecatenary.app/download/linuxDeb) |

Every file, with its SHA-256 checksum, is on the [Releases](https://github.com/GioNicolas/catenary-releases/releases) page. Catenary updates itself after that.

---

## ✨ What's Inside

- **Two lenses, one session** — toggle TerminalMap and Canvas with `Ctrl/Cmd+Alt+S`. Terminals, editors, browsers and dev servers stay alive across the switch.
- **Session cockpit** — one card per work session with your last prompt and the tool the agent is running. The bell rings only when an agent is blocked: an approval, a failure or an explicit request.
- **Splits and Split Zoom** — split the focused terminal right or down (`⌘D` / `⇧⌘D` on macOS, `Alt+Shift+D` / `Alt+Shift+H` on Windows and Linux) and maximize one pane without touching the layout.
- **Agent-aware terminals** — Claude Code, Codex, Antigravity, Cursor, Grok, OpenCode and Pi report when they are working, waiting or done, so you see it without opening the terminal.
- **Agents that talk to each other** — agents in the same session reach each other with `catenary ask`, no copy-paste. On the Canvas, a wire makes the link visible and can relay a finished turn on its own.
- **Maestro Mode** — one agent recruits, briefs and connects a team: 2 helpers on Free, 10 on Pro by default (adjustable from 2 to 50, or unlimited). Recruiting or dismissing an agent stops at a card you approve.
- **Native `catenary mcp` server** — installed agents get `catenary_*` tools automatically: open files, create tasks and worktrees, split terminals, request your attention, delegate work and query the shared LSP.
- **Worktrees for parallel work** — a task gets its own git worktree and branch in one click, with a colour that follows it everywhere.
- **Local and remote take the same path** — point Catenary at a host over SSH or WSL and terminals, git, search and agents run there, while editors, browsers and the canvas stay local.
- **Local-first** — no account and no telemetry: Catenary itself sends nothing. Your agents talk only to their own providers.

---

## 🛠️ Under the Hood

- **Desktop shell:** Electron 41 + Node.js (strict context isolation)
- **Frontend:** React 18, TypeScript, Tailwind CSS
- **Editor:** Monaco (VS Code's editor) + `typescript-language-server` and `pyright`
- **Terminal:** node-pty (native PTY) + xterm.js with the WebGL renderer
- **State:** Zustand + atomic JSON persistence (`.cate/workspace.json`)

---

## 🐞 Bug Reports & Feature Requests

Found a bug or have an idea to make Catenary better?
Please [open an issue](https://github.com/GioNicolas/catenary-releases/issues) or email [support@thecatenary.app](mailto:support@thecatenary.app). You can also send feedback from the app: **Help → Send Feedback…**

---

<div align="center">
  <sub>Engineered by Giorgio Nícolas · <a href="https://thecatenary.app">thecatenary.app</a></sub>
</div>
