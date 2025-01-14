# Usb-Rubber-Ducky-Payloads
Generate Simple Payloads For Rubber Ducky
Here’s an example of a Markdown (`.md`) description for your USB Rubber Ducky encoding tool:

---

# USB Rubber Ducky Encoder Tool

This tool compiles and encodes scripts for USB Rubber Ducky payloads. It supports customizable keyboard layouts and scripting commands, enabling users to craft automated input scripts for various use cases like penetration testing or automation.

## Features

- **Customizable Output Files**: Specify output file paths for encoded payloads.
- **Keyboard Layout Support**: Select from various layouts (e.g., `us`, `es`, `it`, `ru`, etc.).
- **Script Commands**: Write robust input automation scripts using a variety of built-in commands:
  - **ALT**: Execute commands like `ALT F4`, `ALT SPACE`.
  - **CTRL/CONTROL**: Use combinations like `CTRL ESC`, `CTRL-SHIFT ESC`.
  - **GUI/Windows**: Automate GUI actions like `GUI r`.
  - **STRING**: Insert custom text directly as scriptable strings.
  - **DELAY**: Add custom or default delay between commands.
  - **REPEAT**: Loop the last instruction multiple times.
  - And more (`SHIFT`, `REM`, etc.).
  
## Screenshots

![IMG_20250114_233900_485 (2)](https://github.com/user-attachments/assets/863caaec-a8d1-4f79-bc16-594713091a9c)


![Screenshot_20250115-000201](https://github.com/user-attachments/assets/ae84d5ab-5db5-4c18-8fea-99de1c5e9e53)

## Usage

```bash
python3 EvilRubby.py
```

- **Arguments**:
  - `-o [file]`: Output encoded payload to the specified file.
  - `-l [language]`: Set keyboard layout (e.g., `us`, `ru`, `it`).

- **Example Commands**:
  - `ALT F4`: Close the current window.
  - `CTRL ESC`: Open the Start menu.
  - `STRING Hello, World!`: Type "Hello, World!".
  - `DELAY 100`: Pause for 1 second (1000 ms).
  - `REPEAT 5`: Repeat the previous command 5 times.

## Fixes/Improvements

This version has been updated for Python 3 compatibility:
- Replaced `raw_input` with `input`.

## Requirements

- Python 3.x
- `keyboard.properties` file for mapping supported keys.

## Getting Started

1. Clone this repository to your system:
   ```bash
   git clone https://github.com/Iamanyomus/EvilRubby/
   ```
2. Navigate to the encoder directory:
   ```bash
   cd EvilRubby/Encoder
   ```
3. Run the script:
   ```bash
   python3 EvilRubby.py  
   ```
4. Transfer the `payload.bin` to your USB Rubber Ducky device.

