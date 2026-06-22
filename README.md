<div align="center">

# 🤖🔥 HERMES AGENT — YOUR AI COMMAND CENTER 🔥🤖

### 🚀 The Agent That Goes Where You Go — Now in Your Pocket 🚀

[![Android](https://img.shields.io/badge/Android-34A853?logo=android&logoColor=white&style=for-the-badge)](https://play.google.com/store/apps/details?id=hermes.agent.mobile)
[![Play Store](https://img.shields.io/badge/Play_Store-Internal_Testing-414141?logo=googleplay&logoColor=white&style=for-the-badge)](https://play.google.com/store/apps/details?id=hermes.agent.mobile)
[![Status](https://img.shields.io/badge/Status-🔥%20ACTIVE-brightgreen?style=for-the-badge)]()
[![Platform](https://img.shields.io/badge/Platform-Android%20%7C%20Terminal%20%7C%20Desktop-8A2BE2?style=for-the-badge)]()
[![License](https://img.shields.io/badge/License-MIT-FFD700?style=for-the-badge)](LICENSE)

<br />

> **⚡ The Hermes desktop experience — now running natively on Android.**
> **Proot-powered Linux environment. SSH gateway. Agent console. All in one APK.**
> **Your AI agent doesn't sleep. Why should your access to it?**

<br />

```
██████████████████████████████████████████████████████████████████████
██  ██████  █████████████████████████████████████████████████████████
██  ██████  ██████████████████  ██████████  █████████████████████████
██  ██  ██  ██  ████████████████████  ██████████████████████████████
██      ██  ██  ████████████████████  ██████████████████████████████
██  ██████████  ████████████████████████████  ██████████████████████
██  ██████████  ████████████████████████████████████████████████████
██              ████████████████████████████████████████████████████
██████████████████████████████████████████████████████████████████████
██████████████████████████████████████████████████████████████████████
```

</div>

---

## 🤯 What Is This?

**Hermes Agent** is the mobile control surface for serious AI agent workflows. Not a chatbot. Not a toy. A full Linux runtime inside your Android device — with **Proot**, **SSH**, and a **Node.js agent console** — giving you the same power you have on desktop, right from your pocket.

We took the Hermes desktop agent experience and made it **native on Android**. Same agent protocols. Same tool use. Same session history. Same automation. Just... mobile.

**Your agent. Everywhere. Period.**

---

## 📱 Screenshots

<div align="center">
<table>
<tr>
<td align="center" width="33%">
<sub>🤖 Agent Chat</sub>
</td>
<td align="center" width="33%">
<sub>🎛️ Model Switching</sub>
</td>
<td align="center" width="33%">
<sub>📊 Analytics Hub</sub>
</td>
</tr>
<tr>
<td align="center" width="33%">
<sub>📁 File Explorer</sub>
</td>
<td align="center" width="33%">
<sub>🔌 Skill Marketplace</sub>
</td>
<td align="center" width="33%">
<sub>⚙️ Task Manager</sub>
</td>
</tr>
</table>
</div>

> 🔴 *This is not a mockup. This is running on real hardware right now.*

---

## 🌍 What Can You Do With This?

| 🚀 | Capability | What It Means |
|----|------------|---------------|
| 💬 | **Chat with your agent** | Full conversation history, model switching, tool use |
| 🔧 | **Run Linux on Android** | Proot-powered Debian environment — no root needed |
| 🔌 | **SSH into anything** | Built-in SSHd on port 8027, reachable over ADB or network |
| 📁 | **Browse projects** | Navigate repos, files, and workspaces from your phone |
| 🧠 | **Switch models on the fly** | GPT, Claude, Gemini — swap mid-conversation |
| 📊 | **Review analytics** | Usage stats, token tracking, session metrics |
| ⏰ | **Schedule tasks** | Cron-style recurring agent jobs |
| 🛠️ | **Install skills** | Plugin marketplace for extending agent capabilities |
| 🔐 | **Your keys, your control** | BYO API keys, self-hosted or cloud |
| 📱 | **Full mobile UI** | Material Design 3, adaptive layout, edge-to-edge |

---

## ⚡ Quick Start

```bash
# 1. Download from Play Store (internal testing)
#    https://play.google.com/store/apps/details?id=hermes.agent.mobile

# 2. Launch the app

# 3. Connect via ADB or SSH
adb forward tcp:1455 tcp:1455
# Open http://localhost:1455/ in your browser

# Or SSH directly
ssh -p 8027 root@localhost
```

**🎯 And you're flying. Agent empowered. Anywhere.**

---

## 📁 Project Structure

```
📦 hermes-agent-android
├── 🤖 AgentConsole/          # Android app (Compose + Kotlin)
│   ├── app/                  # Main module
│   │   ├── src/main/         # App source
│   │   └── build/            # Generated assets
│   └── install_time_assets/  # Rootfs asset pack (delivered on install)
├── 🌐 playstore/             # Play Store listing & upload scripts
│   ├── upload_to_play.py     # 🚀 Bundle uploader
│   ├── listing/              # Store listing JSON
│   └── screenshots/          # Phone & tablet screenshots
├── 🔧 scripts/               # Build & dev tooling
│   ├── build-rootfs-asset.sh # Rootfs archive builder
│   ├── scrcpy-redroid.sh     # 📱 Tunnel Redroid to your Mac
│   └── mac-play-upload.sh    # macOS upload shortcut
├── 🔌 ssh.sh                 # Quick ADB-SSH wrapper
├── 📖 agents.md              # Full runbook (Docker + Proot SSH)
└── 🔑 play-service-account.json  # Play Console service account
```

---

## 🤖 AgentConsole — The Heart of the App

> *A Kotlin + Jetpack Compose Android app that bundles the Hermes agent runtime into a native APK.*

### 🎯 Key Features

- **🧬 Proot Linux Runtime** — Full Debian environment launched inside the app, no root required
- **🌐 Dashboard Server** — Embedded Node.js HTTP server (agent-console) on port 1455
- **🔌 SSH Gateway** — Proot-based SSHd on port 8027 for terminal access
- **📦 Install-Time Asset Pack** — 600MB+ rootfs delivered via Play Store asset delivery
- **🖼️ Material Design 3** — Adaptive Compose UI with edge-to-edge support
- **🔐 Hermes Upload Keystore** — Signed release builds for Play Store distribution

### 🔧 Build & Deploy

| Command | Output | Target |
|---------|--------|--------|
| `./gradlew :app:assembleRelease` | `app-release.apk` | Local / Redroid testing |
| `./gradlew :app:bundleRelease` | `app-release.aab` | Play Store upload |
| `python3.11 playstore/upload_to_play.py --bundle ...` | 🔄 Internal track release | Internal Testing |

---

## 🔌 SSH Gateway — Why It Matters

> *The SSH gateway is what makes this more than just another mobile app.*

```
┌──────────────┐     ADB forward      ┌────────────┐
│  Your Phone  │ ◄─────────────────── │ Your Laptop │
│  Hermes App  │    tcp:8027:8027      │  Terminal   │
│              │                       │             │
│  ┌────────┐  │                       │ ssh -p 8027 │
│  │ Proot  │  │ ◄─────────────────── │ root@local  │
│  │ SSHD   │  │    SSH session        │  :docker    │
│  └────────┘  │                       │  :automation│
└──────────────┘                       └────────────┘
```

**No cloud dependency. No subscription. Just you, your agent, and your phone.**

---

## 🎯 Requirements

- 📱 **Android 8.0+** (API 26)
- 💾 **1.5GB free storage** (rootfs + app)
- 🧠 **4GB+ RAM recommended** (Proot + Node.js runtime)
- 🔌 **ADB access** for initial setup or SSH tunneling
- 🔑 **API key** for your preferred LLM provider (BYO)

---

## 🐛 Troubleshooting

| Problem | Solution |
|---------|----------|
| ❌ App crashes on launch | Check `adb logcat \| grep -E "proot\|node\|sshd"` for errors |
| 🔇 No audio in scrcpy | Use `--audio-codec=aac` flag |
| 🐢 Slow SSH connection | Ensure ADB forward is active: `adb forward tcp:8027 tcp:8027` |
| 📦 "Missing proot native library" | Build with full APK (includes bundled libs) |
| 🔄 Upload fails | Verify `play-service-account.json` exists and versionCode is bumped |

---

## 🤝 Contributing

This is a fork of [nousresearch/hermes-agent](https://github.com/nousresearch/hermes-agent) adapted for Android. Issues, PRs, and forks welcome.

[![Open Issues](https://img.shields.io/github/issues/phaneron23/hermes-agent?style=for-the-badge&logo=github)](https://github.com/phaneron23/hermes-agent/issues)
[![PRs Welcome](https://img.shields.io/badge/PRs-Welcome-brightgreen?style=for-the-badge)](https://github.com/phaneron23/hermes-agent/pulls)

---

## ⭐ Star This Repo

If you believe your AI agent should be **in your pocket, not in a cloud dashboard** — smash that star button. ⭐

<div align="center">

<a href="https://play.google.com/store/apps/details?id=hermes.agent.mobile">
<img src="https://img.shields.io/badge/📲_GET_IT_ON-PLAY_STORE-34A853?style=for-the-badge&logo=googleplay&logoColor=white" />
</a>

<br /><br />

**Built for the agent-native future** 🔬
*Your agent. Everywhere. Always.* 😏

</div>
*** End Patch
