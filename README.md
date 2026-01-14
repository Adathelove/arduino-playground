# arduino-playground

Persona: Damnameneus

## Blink sketch

- Sketch file: `sketches/blink/blink.ino`
- Board: any Arduino-compatible with `LED_BUILTIN`
- Upload with Arduino IDE or CLI:
  - IDE: File → Open → select `sketches/blink/blink.ino`, pick board/port, Upload.
  - CLI: `arduino-cli compile --fqbn <board_fqbn> sketches/blink && arduino-cli upload -p <serial_port> --fqbn <board_fqbn> sketches/blink`

The sketch toggles `LED_BUILTIN` every 500 ms.
