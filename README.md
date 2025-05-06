# Hack-A-Friend Handheld Gaming Console

### Hone your hacking skills with the **Hack-A-Friend** gaming handheld!  
Delve into epic **CTF attack and defend** style games with your friends. Challenge opponents by **attacking their devices** while defending your own. The winner unleashes a **devastating payload** to dominate their opponent’s game.

---

## 🔥 Features

- **CTF-style gameplay** – Attack and defend devices in real-time battles.
- **Custom payloads** – Winners can craft unique in-game exploits.
- **Open-source** – Clone our upcoming [GitHub repository](#) and create your own games and payloads.
- **Interactive LEDs** – Visual cues for game status and exploit notifications.
- **Bootloader customization** – Recover or modify firmware when needed.

---

## 🔧 Hardware Specifications

- **Power System**:
  - Lithium-ion battery management chip.
  - 500mA LDO for regulated power.
  - Test points for monitoring:
    - `VCC` (battery power source).
    - `3V3` (regulated output from LDO).

- **LED Indicators**:
  - **System notifications**:
    - `PWR` (Power Health LED).
    - `CHG` (Battery Charging LED).
  - **Game Status**:
    - **NeoPixel**:
      - Off – Game idle.
      - Green – Game active.
      - Red – Device under exploitation.
    - **User-Controlled LEDs**:
      - Two standard LEDs for custom exploit visualizations.

- **Debugging & Recovery**:
  - **Test points** for SDA & SCL (I2C debugging with digital signal analyzer).
  - **Bootloader Recovery**:
    - Uses **10-pin ARM TagConnect footprint** (`TC2050-IDC-NL` cable).
    - Compatible with **SWD** and **JTAG** devices like `nRF52840 DK`.
    - Recovery via `nrf-utils` and official bootloader image.
    - **Segger J-Link compatibility
