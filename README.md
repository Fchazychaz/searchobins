# searchobins

`searchobins` is a Bash-based helper tool that allows you to quickly search **GTFOBins** payloads directly from the terminal.

It is designed for **Hack The Box**, **CTFs**, and **pentesting workflows**, helping you quickly retrieve payloads and descriptions for binaries without opening the browser.

---

## 🚀 Features

- Search payloads by binary and function
- Display a short explanation of the technique
- List all available functions for a binary
- Colored terminal output
- Lightweight Bash script
- Ideal for HTB / CTFs

---

## 📦 Installation

Clone the repository:

```bash
git clone https://github.com/Fchazychaz/searchobins.git
cd searchobins
chmod +x searchobins
sudo mv searchobins /usr/local/bin/
```

---

## 🔍 Usage

### Search for a specific payload

```bash
searchobins -b python -f shell
```

Example output:

```text
[+] Explanation:
This executable can spawn an interactive system shell.

[+] Payload:
python -c 'import os; os.system("/bin/sh")'
```

---

### List available functions

```bash
searchobins -b python -l
```

Example output:

```text
shell
reverse-shell
file-read
file-write
sudo
library-load
```

---

## 🛠 Options

| Option | Description |
|--------|-------------|
| `-b` | Binary name |
| `-f` | Function name |
| `-l` | List available functions |
| `-h` | Show help panel |

---

## 📚 Examples

```bash
searchobins -b pip -f shell
searchobins -b tar -f sudo
searchobins -b python -l
```

---

## 🎯 Use cases

Perfect for:

- Hack The Box
- CTF competitions
- Privilege escalation
- File read/write techniques
- Quick shell spawning

---

## 🤝 Contributing

Contributions, ideas and improvements are welcome.

Feel free to fork the project and submit a pull request.

---

## ⚠️ Disclaimer

This tool is intended for **educational purposes and authorized security testing only**.

Use responsibly.

---

## 👨‍💻 Author

Created by **Fchazychaz**
