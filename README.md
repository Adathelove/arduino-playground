# arduino-playground

Persona: Damnameneus

## Blink sketch

- Sketch file: `sketches/blink/blink.ino`
- Board: any Arduino-compatible with `LED_BUILTIN`
- Upload with Arduino IDE or CLI:
  - IDE: File → Open → select `sketches/blink/blink.ino`, pick board/port, Upload.
  - CLI: `arduino-cli compile --fqbn <board_fqbn> sketches/blink && arduino-cli upload -p <serial_port> --fqbn <board_fqbn> sketches/blink`

The sketch toggles `LED_BUILTIN` every 500 ms.

## PlatformIO setup (classic Arduino/Uno)

- Config: `platformio.ini` with `[env:uno]` (platform `atmelavr`, board `uno`, framework `arduino`, monitor 9600).
- Source: `src/main.cpp` (same blink code).
- In VS Code with PlatformIO extension:
  - Open this folder, let PIO install the toolchain.
  - Use the status bar buttons: Build → Upload → Monitor.
  - If your board isn’t an Uno, change `board = <id>` in `platformio.ini` (e.g., `nanoatmega328`, `megaatmega2560`, `teensy41`).
