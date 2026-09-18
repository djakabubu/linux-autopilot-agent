## 🎉 Linux Autopilot Agent v1.0.0

**An interactive AI agent for Linux system administration, debugging and automation — powered by OpenRouter.**

This is the first public release of **Linux Autopilot Agent**, a terminal-based assistant that lets you control a Linux machine (including Raspberry Pi) in natural language.

---

### ✨ Highlights

- 🗣️ **Natural language control** — describe what you want in plain English.
- 🛡️ **Local risk engine** — commands are classified as `SAFE`, `CAUTION` or `DANGEROUS` by deterministic rules that run locally, independent of the model.
- ✅ **Auto-execution of safe commands** — read-only and harmless operations run without asking.
- ⚠️ **Interactive confirmation** — only for destructive, privileged, network, system or potentially exfiltrating operations.
- 🔒 **Secret redaction** — API keys, tokens, passwords and private keys are scrubbed from output before it reaches the model.
- 📦 **Zero dependencies** — pure Python standard library, no `pip install` needed.
- 🔄 **Streaming responses** — see the model's reasoning and output in real time.
- 💾 **Persistent history** — requests saved to `history.json` next to the script.
- 🧩 **Multi-model support** — switch models on the fly with `:model`.
- 🤖 **Autopilot mode** — run everything without confirmation (use with care).

---

### 🚀 Quick Start

```bash
# 1. Set your OpenRouter API key
export OPENROUTER_API_KEY='sk-or-v1-...'

# 2. Run interactively
python3 linux_autopilot.py

# Or run a one-shot task
python3 linux_autopilot.py "check why docker won't start"
```

---

### 🛠️ Installation

```bash
git clone https://github.com/djakabubu/linux-autopilot-agent.git
cd linux-autopilot-agent
chmod +x linux_autopilot.py
```

No `pip install` required — the agent uses only the Python standard library.

---

### 📄 License

This project is licensed under the **MIT License**.

---

⭐ If you find this useful, please consider giving it a star!