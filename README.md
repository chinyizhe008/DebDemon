# 🐍 DebDemon – The Stealthy Debian Rootkit

[![PyPI Version](https://img.shields.io/pypi/v/debdemon.svg?color=orange&label=PyPI)](https://pypi.org/project/debdemon)
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![GitHub Stars](https://img.shields.io/github/stars/yourname/debdemon.svg?style=social)](https://github.com/yourname/debdemon/stargazers)

**DebDemon** is a *fully undetectable (FUD)* rootkit for Debian-based Linux. It stealthily hides processes, files, and connections while giving you root-level access. Ideal for red teaming and research. 👹🔒

---
# 📁 Project Structure
- debdemon/
- ├── core/
- │   ├── preload_hider.c       # LD_PRELOAD rootkit core
- │   └── loader.py             # Python wrapper for deploying .so
- ├── plugins/
- │   ├── reverse_shell.py      # Encrypted reverse shell plugin
- │   └── __init__.py
- ├── cli/
- │   └── daemon.py             # Backdoor CLI trigger logic
- ├── setup.py
- ├── debdemon.py               # Main bootstrap
- └── README.md



## 📚 Table of Contents

- [🎯 Features](#-features)
- [⚙️ Installation](#-installation)
- [🚀 Usage](#-usage)
- [🛑 Disclaimer](#-disclaimer)
- [🤝 Contributing](#-contributing)
- [🧾 License](#-license)

---

## 🎯 Features

- 👻 Ghost mode: Hide processes, users, and open ports from system tools.
- 🔁 Persistence: Stays active across reboots via hidden services.
- 🔌 Modular: Supports plugins for reverse shells, sniffers, and more.
- 💡 Configurable CLI: Access and configure via a hidden command-line interface.

---

## ⚙️ Installation

Install via pip (coming soon):

```bash
pip install debdemon
