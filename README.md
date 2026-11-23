# MuteMe

Minimalist Windows tray utility to mute and unmute the default microphone via a global hotkey.

## Features
- **Global hotkey** — works across any active window or fullscreen application (`F9` by default).
- **Tray integration** — runs in the system tray with an icon reflecting current microphone status (live or muted).
- **Custom keybinds** — change and save hotkeys directly in the interface.
- **Background execution** — runs without a console window.
- **Single instance** — prevents duplicate processes via Windows named mutex.

## Installation
Download `MuteMe.exe` from the [Releases](../../releases) page and run it. No Python installation is required.

*Note: Since the executable is unsigned, Windows SmartScreen may show a warning. Click **More info** -> **Run anyway**.*

## Building from Source
1. Install dependencies:
   ```bash
   pip install customtkinter keyboard pillow pycaw comtypes pystray
   ```

2. Run without building:
   ```bash
   pythonw muteme.pyw
   ```

3. Build standalone executable:
   ```bash
   pyinstaller --noconfirm --onefile --windowed --icon="muteme.ico" --add-data "muteme.ico;." --collect-all customtkinter --name "MuteMe" muteme.pyw
   ```

## Configuration
Settings and error logs are stored locally in `%APPDATA%\MuteMe\`.

## License
[MIT](LICENSE)

## MicMute
<img width="159" height="193" alt="{8D670972-D3C6-4349-B096-86731274DF65}" src="https://github.com/user-attachments/assets/fec20a18-4f4f-4716-8215-fdf10dbd5ec3" />
|
<img width="292" height="338" alt="{E4CF6AD1-5195-4181-8E50-9080C471A01C}" src="https://github.com/user-attachments/assets/713cf88d-1997-4fd0-85ea-651e4ce0529a" />
