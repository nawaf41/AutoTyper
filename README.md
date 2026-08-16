# Auto Typer

A lightweight Windows macro tool that simulates keystrokes into whatever window currently has focus. Works in any application that accepts keyboard input — text editors, games, chat apps, forms, and more.

## Features

- **Message list** — type multiple messages, sent in order or picked randomly
- **Loop control** — repeat a set number of times, or run indefinitely until stopped
- **Custom delay per line** — override the global interval for any specific message
- **Adjustable typing speed** — instant to human-like
- **Presets** — save and reload your message lists and settings
- **Hotkeys** — fully customizable Start / Pause / Resume / Stop / Emergency Stop
- **Run history** — see past runs (time, messages sent, duration)
- **Dark / light themes**
- **Compact mode** — collapse extra panels down to just the essentials
- **Safety checks** — warns before infinite loops or very fast intervals, and won't run if the app itself is still focused

## Download

Grab the latest `AutoTyper.exe` from the [Releases](../../releases) page. No installation, no Python required — just download and run.

## How it works

Auto Typer simulates real keystrokes at the operating system level, the same as if you were typing manually. Click into the window you want to type into, then either:

- Click **Start** in the app (gives you a 3-second countdown to switch windows), or
- Press the **Start hotkey** (default `F8`) while already focused on your target window — it sends immediately, no countdown

## Building from source

```bash
pip install pyautogui keyboard pyinstaller
pyinstaller --onefile --windowed --name AutoTyper --icon=icon.ico main.py
```

The finished executable will be in `dist/AutoTyper.exe`.

## Requirements to run from source

- Python 3.10+
- `pyautogui`
- `keyboard`

## License

MIT

---

⭐ If you find this useful, consider starring the repo.
🔗 [More projects](https://github.com/nawaf41)
