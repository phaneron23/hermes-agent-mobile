<div align="center">

# 🤖🔥 Hermes Agent Mobile 🔥🤖

### 🚀 Your AI Agent, Fully Local on Android — or Remotely Connected to Your Existing Hermes Instance 🚀

[![Play Store](https://img.shields.io/badge/Play%20Store-Hermes%20Agent%20Mobile-34A853?style=for-the-badge&logo=googleplay&logoColor=white)](https://play.google.com/store/apps/details?id=hermes.agent.mobile)
[![Latest APK](https://img.shields.io/badge/Latest%20APK-Direct%20Download-ffb000?style=for-the-badge&logo=android&logoColor=white)](https://github.com/phaneron23/hermes-agent-mobile/releases/latest/download/app-release.apk)
[![GitHub Pages](https://img.shields.io/badge/Website-Live-8A2BE2?style=for-the-badge&logo=githubpages&logoColor=white)](https://phaneron23.github.io/hermes-agent-mobile/)
[![Android](https://img.shields.io/badge/Platform-Android-3DDC84?style=for-the-badge&logo=android&logoColor=white)](https://play.google.com/store/apps/details?id=hermes.agent.mobile)
[![Status](https://img.shields.io/badge/Status-Internal%20Testing-FF6B35?style=for-the-badge)](https://play.google.com/store/apps/details?id=hermes.agent.mobile)

<br />

> **Hermes Agent Mobile is the pocket command center for Hermes.**
>
> Run the whole agent stack locally on Android, or connect to an existing Hermes instance running somewhere else.
>
> **Local when you want sovereignty. Remote when you want reach. Mobile always.**

<br />

```
╔══════════════════════════════════════════════════════════════╗
║                 H E R M E S   A G E N T                    ║
║                        M O B I L E                         ║
║                                                              ║
║        LOCAL LINUX RUNTIME  •  REMOTE HERMES CONTROL        ║
╚══════════════════════════════════════════════════════════════╝
```

</div>

---

## 🧠 TL;DR

**Hermes Agent Mobile** gives you two powerful modes:

- **📱 Fully Local Mode** — run Hermes directly on Android with a bundled Linux runtime, Node.js agent console, Proot, and SSH gateway.
- **🌐 Remote Control Mode** — connect the mobile app to an existing Hermes instance on your desktop, server, cloud VM, or private homelab.

Same vibe. Same agent. Different gravity.

---

## 🤯 What Is This?

Hermes Agent Mobile is not just another chatbot shell. It is a mobile-first control surface for real agent workflows: conversations, model routing, tools, files, tasks, SSH, and automation.

Want everything self-contained? Run the agent stack locally on Android.

Already have Hermes running on a beefy machine? Connect remotely and use your phone as the cockpit.

**Yes, that means local autonomy. Yes, that means remote power. Yes, that means your agent finally follows you outside the desk cave.**

---

## 🚀 Two Modes, One Agent

| Mode | Best For | What Happens |
|---|---|---|
| 📱 **Fully Local** | Offline experiments, portable autonomy, Android-first hacking | The app launches a local Linux runtime and agent console directly on-device. |
| 🌐 **Remote Hermes** | Desktop/server workflows, bigger models, long-running jobs | The app connects to an existing Hermes instance and becomes your mobile command center. |

---

## 🌍 What Can You Do With It?

| 🔥 | Capability | Why It Matters |
|---|---|---|
| 💬 | **Chat with your agent** | Keep working from your phone without losing context. |
| 🐧 | **Run locally on Android** | Proot-powered Linux runtime without rooting your device. |
| 🌐 | **Connect remotely** | Control an existing Hermes instance from anywhere. |
| 🔌 | **Use SSH workflows** | Terminal access for debugging, scripts, and deeper control. |
| 📁 | **Browse projects** | Inspect files, repos, and workspace state on the move. |
| 🧠 | **Switch models** | Route work to the right model for the job. |
| ⚙️ | **Manage tasks** | Launch, monitor, and resume agent work. |
| 🔐 | **Bring your own keys** | Keep auth and provider choices under your control. |
| 📊 | **Review usage** | See sessions, costs, and activity without opening a laptop. |

---

## 📲 Get Hermes Agent Mobile

<div align="center">

[![Get Hermes Agent Mobile on Play Store](https://img.shields.io/badge/GET%20IT%20ON-GOOGLE%20PLAY-34A853?style=for-the-badge&logo=googleplay&logoColor=white)](https://play.google.com/store/apps/details?id=hermes.agent.mobile)
[![Download Latest APK](https://img.shields.io/badge/DOWNLOAD-LATEST%20APK-ffb000?style=for-the-badge&logo=android&logoColor=white)](https://github.com/phaneron23/hermes-agent-mobile/releases/latest/download/app-release.apk)

</div>

Play Store package:

```text
hermes.agent.mobile
```

Latest APK:

```text
https://github.com/phaneron23/hermes-agent-mobile/releases/latest/download/app-release.apk
```

---

## ⚡ Quick Start

### 📱 Fully Local Mode

```bash
# Install from Play Store
# Launch Hermes Agent Mobile
# Let the bundled runtime start
# Open the local dashboard or connect over SSH
```

### 🌐 Remote Hermes Mode

```bash
# Point the app at your existing Hermes instance
# Connect from Android
# Keep working from your phone
```

### 🔌 Local Debug Access

```bash
# Dashboard
adb forward tcp:1455 tcp:1455
open http://localhost:1455/

# SSH gateway
adb forward tcp:8027 tcp:8027
ssh -p 8027 root@localhost
```

---

## 🏗️ Architecture

```text
┌───────────────────────────────────────────────────────┐
│                 Hermes Agent Mobile                   │
│                                                       │
│  ┌───────────────────────┐    ┌────────────────────┐  │
│  │  📱 Local Mode         │    │  🌐 Remote Mode     │  │
│  │                       │    │                    │  │
│  │  Proot Linux Runtime  │    │  Existing Hermes   │  │
│  │  Node Agent Console   │    │  Desktop / Server  │  │
│  │  SSH Gateway          │    │  Cloud / Homelab   │  │
│  └───────────┬───────────┘    └─────────┬──────────┘  │
│              │                          │             │
│              └──────── Mobile UI ───────┘             │
│                                                       │
│              Chat • Files • Models • Tasks            │
└───────────────────────────────────────────────────────┘
```

---

## 🧩 Why This Exists

Because agents should not be trapped behind a desktop window.

Because sometimes the right computer is the server, sometimes it is the phone, and sometimes it is both.

Because the future is not “one app.” It is **one agent surface across every machine you own**.

---

## ⭐ Star This Repo

If you believe your AI agent should run **locally**, connect **remotely**, and stay **with you** — star the repo and grab the Android build.

<div align="center">

[![Open Website](https://img.shields.io/badge/Open-Website-8A2BE2?style=for-the-badge&logo=githubpages&logoColor=white)](https://phaneron23.github.io/hermes-agent-mobile/)
[![Play Store](https://img.shields.io/badge/Open-Play%20Store-34A853?style=for-the-badge&logo=googleplay&logoColor=white)](https://play.google.com/store/apps/details?id=hermes.agent.mobile)
[![Latest APK](https://img.shields.io/badge/Open-Latest%20APK-ffb000?style=for-the-badge&logo=android&logoColor=white)](https://github.com/phaneron23/hermes-agent-mobile/releases/latest/download/app-release.apk)

<br />

**Hermes Agent Mobile** — *local power, remote reach, pocket-sized chaos.* 😏

</div>
