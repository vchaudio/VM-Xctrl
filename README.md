![Banner](https://public-files.gumroad.com/ahv3hxr873cmpl3dor9kq635l0kv)

# VM-XCtrl  
**Voicemeeter ↔ Behringer X-Touch Bridge**

**VM-XCtrl** bridges the **Behringer X-Touch** control surface with **VB-Audio Voicemeeter**, providing tactile control, visual feedback, and powerful layer-based mixing.  
It communicates via **UDP** in **XCtrl mode**, using the **Voicemeeter API** to synchronize faders, buttons, displays, and meters.

## Overview
VM-XCtrl maps the X-Touch’s **faders, buttons, encoders, and scribble displays** directly to Voicemeeter’s parameters.  
You get hands-on mixing, real-time feedback, and advanced features like AUX (send) control, preset recall, and media transport — all from your X-Touch.

A key advantage is that you can run the X-Touch in **XCtrl/MCU mode**, keeping **Voicemeeter** on one layer and your **DAW or other software** on another, easily switched via the **SMPTE** button.

## Features v.1.0
- Two main layers:  
  - **Input Layer** controls Voicemeeter strips (channels)  
  - **Output Layer** controls buses  
  Switch seamlessly between them.  
- **9 faders total:** 8 channel faders + 1 master fader on the Input layer.  
- **Full channel metering bars:** real-time LED meters synced to Voicemeeter levels.  
- **Dynamic scribble strips:**  
  - Line 1 shows channel labels  
  - Line 2 shows labels or live gain values (in dB) when touching a fader  
  - Distinct color palettes for Input, Output, and AUX layers.  
- **Button feedback:** Mute, Solo, Mono, and M.C toggles mirror Voicemeeter’s state with LED feedback.  
- **AUX (Send) layer:**  
  - Accessed by selecting a channel  
  - Control send levels for A1–A5 and B1–B3  
  - Displays indicate active buses with color feedback  
  - Dedicated RECORD buttons toggle sends  
  - Meters show input gain for the selected channel and relative levels for active sends  
- **Preset recall:** F1–F8 keys instantly recall Voicemeeter presets with LED feedback.  
- **Media transport controls:** Play, pause, next, and previous buttons send OS-level media keys, with illuminated LEDs to indicate playback state.  
- **Reliable communication:**  
  - Robust UDP handshake and keep-alive between X-Touch and VM-XCtrl  
  - Automatic connection loss detection and recovery  
  - “DISCONNECTED API” layer appears when Voicemeeter is offline, returning automatically once reconnected  
- **FLIP button:** toggles fader mode (Absolute / Relative).  
- **Solo feedback:** when a channel is soloed, other mute LEDs blink — identical to Voicemeeter’s visual behavior.  
- **Layer display:** in single XCtrl mode, the display shows the current layer name (Bars, Beats, Subdivision, or Ticks fields repurposed).

## Video Preview

[![Video Preview](https://img.youtube.com/vi/OcrzrS9EKOE/0.jpg)](https://www.youtube.com/watch?v=OcrzrS9EKOE)

## Requirements
- **VB-Audio Voicemeeter** (Potato - 3.1.1.9 / Banana - 2.1.1.9 / or higher)  
- **Behringer X-Touch** (XCtrl / XCtrl-MCU / XCtrl-HUI mode)  
- **UDP network access** — PC and X-Touch must be on the same local network

## Getting Started
1. Connect your **Behringer X-Touch** in **XCtrl** mode.  
2. Launch **Voicemeeter** and ensure the API is enabled.  
3. Run **VM-XCtrl** — it will automatically detect and connect.
4. Assign X-Touch IP
5. Assign PC IP on X-Touch (hover your mouse on the tray icon, it will show you your IP)
6. Control Voicemeeter directly from your X-Touch.

Get your Licence Key
https://vchaudio.gumroad.com/l/VM-XCtrl


Leave Feedback and stay tuned on the official Discord server 
[https://discord.gg/DzCBwq2e](https://discord.gg/jyh8bSUev7)

