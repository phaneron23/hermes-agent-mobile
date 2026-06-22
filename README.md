<div align="center">

# 🤖🔥 HERMES AGENT 🔥🤖

### 🚀 The Agent That Goes Where You Go — Now in Your Pocket 🚀

[![Play Store](https://img.shields.io/badge/📲_Get_it_on-Play_Store-34A853?style=for-the-badge&logo=googleplay&logoColor=white)](https://play.google.com/store/apps/details?id=hermes.agent.mobile)
[![Android](https://img.shields.io/badge/Platform-Android-34A853?style=for-the-badge&logo=android&logoColor=white)]()
[![Status](https://img.shields.io/badge/Status-Internal_Testing-FF6B35?style=for-the-badge)]()
[![License](https://img.shields.io/badge/License-MIT-FFD700?style=for-the-badge)](LICENSE)

<br />

> **⚡ Your AI agent — now in your pocket.**
>
> Proot-powered Linux runtime. SSH gateway. Agent console.
>
> **Desktop power. Mobile freedom.**

</div>

---

## 🤯 What Is This?

**Hermes Agent** is a native Android app that puts a full AI agent runtime in your pocket.

Not a chatbot wrapper. Not a cloud UI. A real Linux environment (Proot), a Node.js agent server, and a full SSH gateway — all inside a single APK.

- 💬 Chat with your agent on the go
- 🔧 Run Linux commands on your phone — no root required
- 🔌 SSH into your agent from any device
- 📁 Browse repos, projects, and files from mobile
- 🧠 Switch LLM models mid-conversation
- ⏰ Schedule automated agent tasks

**Your agent. Everywhere. Always.**

---

## 📱 Get It

<div align="center">
  <a href="https://play.google.com/store/apps/details?id=hermes.agent.mobile">
    <img src="https://img.shields.io/badge/📲_DOWNLOAD_FROM-PLAY_STORE-34A853?style=for-the-badge&logo=googleplay&logoColor=white" />
  </a>
</div>

> Currently in **Internal Testing** — new builds shipped regularly.

---

## ⚡ Quick Start

```bash
# 1. Install from Play Store
# 2. Connect via ADB

adb forward tcp:1455 tcp:1455
# Open http://localhost:1455/ in your browser

# Or SSH directly into the agent
adb forward tcp:8027 tcp:8027
ssh -p 8027 root@localhost
```

---

## 🏗️ Architecture

```
┌─────────────────────────────────────┐
│         📱 Hermes App (APK)         │
│  ┌───────────────────────────────┐  │
│  │  🤖 Agent Console (Node.js)   │  │
│  │  🌐 Dashboard :1455           │  │
│  │  🔌 SSH Gateway :8027         │  │
│  └──────────┬────────────────────┘  │
│  ┌──────────▼────────────────────┐  │
│  │  🐧 Proot Linux Runtime       │  │
│  │  📦 Full Debian rootfs        │  │
│  │  🔧 Python, Node, git, etc.   │  │
│  └───────────────────────────────┘  │
└─────────────────────────────────────┘
```

---

## 🎯 Features

|  | Feature | What It Does |
|---|---|---|
| 💬 | Agent Chat | Full conversation with tool use, memory, and model switching |
| 🐧 | Linux Runtime | Proot-powered Debian — no root, no cloud |
| 🔌 | SSH Gateway | SSHd at port 8027 — access from laptop, desktop, or another phone |
| 🌐 | Web Dashboard | Built-in HTTP server on port 1455 |
| 📁 | File Management | Browse repos, read files, edit configs |
| 🧠 | Multi-Model | GPT, Claude, Gemini — swap mid-conversation |
| 📊 | Analytics | Token usage, session history, agent metrics |
| 🔐 | Your Keys | BYO API keys — self-hosted or cloud |
| 📱 | Native UI | Material Design 3, edge-to-edge, adaptive layout |

---

## 📦 What's Inside

| Component | Description |
|---|---|
| `AgentConsole/` | Android app (Kotlin + Jetpack Compose) |
| `install_time_assets/` | Rootfs delivered via Play Asset Delivery |
| `playstore/` | Upload scripts and store listing |
| `scripts/` | Build and dev tooling |

---

## 🛠️ Build

```bash
# APK for local testing
./gradlew :app:assembleRelease

# AAB for Play Store
./gradlew :app:bundleRelease

# Upload to internal track
python3 playstore/upload_to_play.py \
  --package hermes.agent.mobile \
  --bundle app/build/outputs/bundle/release/app-release.aab \
  --service-account play-service-account.json \
  --track internal
```

---

## 🤝 Contributing

This is an Android adaptation of [nousresearch/hermes-agent](https://github.com/nousresearch/hermes-agent).

PRs, issues, and forks welcome.

---

## ⭐ Star This Repo

**If your agent should be in your pocket — not in a cloud dashboard — smash that star.** ⭐

<div align="center">
  <a href="https://play.google.com/store/apps/details?id=hermes.agent.mobile">
    <img src="https://img.shields.io/badge/📲_GET_IT_ON-PLAY_STORE-34A853?style=for-the-badge&logo=googleplay&logoColor=white" />
  </a>

  <br /><br />

  *Your agent. Everywhere. Always.* 😏
</div>
