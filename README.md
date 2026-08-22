# Termux-Objection-Frida
🔥 How to Install Objection & Frida in Termux


🔥 How to Install Objection & Frida in Termux

<p align="center">
  <img src="https://img.shields.io/badge/Termux-000000?style=for-the-badge&logo=android&logoColor=white">
  <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white">
  <img src="https://img.shields.io/badge/Frida-E53935?style=for-the-badge">
  <img src="https://img.shields.io/badge/Objection-8E44AD?style=for-the-badge">
</p><p align="center">
  <b>⚡ Professional Frida & Objection installation guide for Termux</b>
</p>---

📋 Requirements

- 📱 Android device
- 💻 Termux
- 🌐 Internet connection
- 🐍 Python

---

🚀 Installation

🟢 1. Update Termux & Install Python

apt update && apt upgrade && apt install python

---

🔴 2. Install Frida

apt install frida-python

Check the installation:

frida --version

---

🟣 3. Install Objection Dependencies

pip install click delegator-py flask litecli packaging prompt-toolkit pygments requests semver setuptools tabulate

---

⚡ 4. Install Objection

pip install objection --no-deps

Check the installation:

objection --version

---

🎯 Quick Installation

apt update && apt upgrade && apt install python

apt install frida-python

pip install click delegator-py flask litecli packaging prompt-toolkit pygments requests semver setuptools tabulate

pip install objection

---

🔍 Verify Installation

🐍 Python

python --version

🔥 Frida

frida --version

🟣 Objection

objection --version

📦 Installed Packages

pip list

---

🧩 Dependencies

Package| Description
🖱️ "click"| Command-line interface toolkit
⚙️ "delegator-py"| Shell command execution
🌐 "flask"| Python web framework
🗄️ "litecli"| SQLite command-line client
📦 "packaging"| Python package utilities
⌨️ "prompt-toolkit"| Interactive CLI interfaces
🎨 "pygments"| Syntax highlighting
🌐 "requests"| HTTP requests
🔢 "semver"| Semantic versioning
🛠️ "setuptools"| Python packaging
📊 "tabulate"| Pretty terminal tables

---

🛠️ Troubleshooting

❌ "pip: command not found"

python -m pip --version

If necessary:

apt update

apt install --reinstall python

Then:

python -m pip --version

🔎 Find Installation Paths

which python

which pip

which frida

which objection

📦 Check Objection

python -m pip show objection

🔥 Check Frida

python -m pip show frida

---

🧪 Test Python Imports

Frida

python -c "import frida; print(frida.__version__)"

Objection

python -c "import objection; print('Objection imported successfully')"

---

📊 Check Versions

python --version && frida --version && objection --version

---

⚠️ Compatibility

If you encounter "ModuleNotFoundError", "ImportError", or version conflicts, check:

python --version

frida --version

objection --version

pip list

Make sure your Frida-related packages and Objection version are compatible.

---

👨‍💻 Credits

<p align="center">
  <b>Created by Josif Khan</b>
</p><p align="center">
  🐙 <b>GitHub:</b> <a href="https://github.com/josifkhang">@josifkhang</a>
  <br>
  ✈️ <b>Telegram:</b> <a href="https://t.me/josifkhan">@josifkhan</a>
</p>---

⚖️ Disclaimer

This guide is intended for authorized security research, application testing, debugging, and educational purposes.

Only use Frida and Objection on applications and devices that you own or have explicit permission to test.

---

<p align="center">
  <b>⭐ Star the repository if this guide helped you!</b>
  <br><br>
  Made with ❤️ by <b>Josif Khan</b>
</p>
