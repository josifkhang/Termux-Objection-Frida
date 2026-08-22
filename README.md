# Termux-Objection-Frida
How to install objection and frida in termux

🔥 How to Install Objection & Frida in Termux

<p align="center">
  <img src="https://img.shields.io/badge/Platform-Termux-black?style=for-the-badge&logo=android" alt="Termux">
  <img src="https://img.shields.io/badge/Python-3.x-blue?style=for-the-badge&logo=python" alt="Python">
  <img src="https://img.shields.io/badge/Frida-Ready-red?style=for-the-badge" alt="Frida">
  <img src="https://img.shields.io/badge/Objection-Ready-purple?style=for-the-badge" alt="Objection">
</p><p align="center">
  <b>⚡ A clean and professional guide for installing Frida & Objection on Termux.</b>
</p>---

📋 Requirements

Before starting, make sure you have:

- 📱 Android device
- 💻 Termux
- 🐍 Python 3
- 🌐 Internet connection

«⚠️ Important: Use the official/current Termux distribution rather than outdated Play Store builds.»

---

🚀 Installation

🟢 Step 1 — Update Termux & Install Python

apt update && apt upgrade && apt install python

---

🔵 Step 2 — Install Frida

Install the Frida Python package:

apt install frida-python

Verify the installation:

frida --version

Expected output:

17.x.x

«Your exact version may be different.»

---

🟣 Step 3 — Install Objection Dependencies

Install the required Python packages:

pip install click delegator-py flask litecli packaging prompt-toolkit pygments requests semver setuptools tabulate

---

🔴 Step 4 — Install Objection

Install Objection using pip:

pip install objection --no-deps

Verify:

objection --version

You can also check:

objection --help

---

⚡ One-Command Setup

If your Termux Python environment is already working, you can install the required components with:

apt update && apt upgrade && apt install python frida-python && \
pip install click delegator-py flask litecli packaging prompt-toolkit pygments requests semver setuptools tabulate && \
pip install objection

---

🔍 Verify Everything

Check Python

python --version

Check pip

python -m pip --version

Check Frida

frida --version

Check Objection

objection --version

Check installed packages

pip list

---

🧩 Dependencies

📦 Package| 🔧 Purpose
"click"| CLI framework
"delegator-py"| Command execution
"flask"| Web framework
"litecli"| SQLite CLI
"packaging"| Package/version utilities
"prompt-toolkit"| Interactive terminal UI
"pygments"| Syntax highlighting
"requests"| HTTP requests
"semver"| Semantic versioning
"setuptools"| Python packaging
"tabulate"| Formatted tables

---

🛠️ Troubleshooting

❌ "pip: command not found"

Try:

python -m pip --version

If Python is installed but pip is unavailable, reinstall/update the Termux Python package:

apt update
apt install --reinstall python

Then check:

python -m pip --version

---

❌ Check where packages are installed

python -m pip show objection

For Frida:

python -m pip show frida

---

❌ Show all packages installed

python -m pip list

Or:

python -m pip freeze

---

📁 Useful Commands

which python
which pip
which frida
which objection

Check Python executable:

python -c "import sys; print(sys.executable)"

Check Frida import:

python -c "import frida; print(frida.__version__)"

Check Objection import:

python -c "import objection; print('Objection imported successfully')"

---

⚠️ Compatibility

Frida, Objection, Python, and Termux package versions must be compatible.

If you encounter an error such as:

ModuleNotFoundError

or:

ImportError

check the installed versions first:

python --version
frida --version
objection --version
pip list

---

🎯 Quick Reference

┌─────────────────────────────────────────────┐
│              TERMUX SETUP                   │
├─────────────────────────────────────────────┤
│                                             │
│  🐍 Python       → apt install python       │
│  🔥 Frida        → apt install frida-python │
│  🟣 Dependencies → pip install ...          │
│  ⚡ Objection    → pip install objection     │
│                                             │
└─────────────────────────────────────────────┘

---

⭐ Credits

<p align="center">
  <b>Built for Termux users ⚡</b><br>
  Frida + Objection + Python
</p><p align="center">
  <img src="https://img.shields.io/badge/Made%20with-Termux-00C853?style=for-the-badge&logo=android" alt="Made with Termux">
</p>---

⚖️ Disclaimer

This guide is intended for authorized security research, application testing, debugging, and educational purposes. Only instrument applications and devices that you own or have explicit permission to test.
