# VM-XCtrl

<p align="center">
  <img width="3840" height="1098" alt="VM-XCtrl" src="https://github.com/user-attachments/assets/22eae376-653a-4186-86a5-151345483ec8" />
</p>

<p align="center">
  <strong>VoiceMeeter X-Touch Control Bridge</strong><br>
  Turn your Behringer X-Touch into a complete VoiceMeeter and Windows mixing console.
</p>

<p align="center">
  <a href="https://github.com/vchaudio/VM-XCtrl/releases"><img src="https://img.shields.io/github/v/release/vchaudio/VM-XCtrl?style=for-the-badge&label=Release&labelColor=172B3A&color=FF5A1F&logo=github&logoColor=white"></a>
  <a href="#-requirements"><img src="https://img.shields.io/badge/Windows-10%20%7C%2011-FF5A1F?style=for-the-badge&logo=windows&logoColor=white&labelColor=172B3A"></a>
  <a href="#-requirements"><img src="https://img.shields.io/badge/Connection-LAN%20%7C%20USB%20%7C%20MIDI-3D8BC9?style=for-the-badge&labelColor=172B3A"></a>
  <a href="#-license"><img src="https://img.shields.io/badge/License-Proprietary%20%2F%20Commercial-FACC15?style=for-the-badge&labelColor=172B3A"></a>
</p>

<p align="center">
  <strong>Requirements:</strong><br>
  Windows 10/11 · VoiceMeeter Potato or Banana · Behringer X-Touch · LAN/USB/MIDI connection
</p>


## 📦 What is VM-XCtrl?
>[!NOTE]
>VM-XCtrl is a native Windows application that connects **VoiceMeeter Potato / Banana** with the **Behringer X-Touch** over LAN, MIDI, and USB.
It communicates directly with the VoiceMeeter API and translates its controls and state into the **XCtrl or Mackie protocol**.
The entire X-Touch layout is purpose-built for VoiceMeeter. No MIDI mapping, button assignment, or manual control setup is required.
The result is a ready-to-use **hardware mixing console for Windows**, combining VoiceMeeter mixing, Windows application control, media control, and hardware routing on a single X-Touch.

<p align="center">
  <a href="https://www.youtube.com/watch?v=OcrzrS9EKOE">
    <img src="https://img.shields.io/badge/▶%20Presentation Video-FF0000?style=for-the-badge&logo=youtube&logoColor=white">
  </a>
</p>

## 📚 Table of Contents
- [X-Touch Modes](#-x-touch-modes)
- [Features](#%EF%B8%8F-features)
  - [INPUT Layer](#%EF%B8%8F-features)
  - [OUTPUT Layer](#%EF%B8%8F-features)
  - [SEND Layer](#%EF%B8%8F-features)
  - [APPs Layer](#%EF%B8%8F-features)
- [Additional Features](#-additional-features)
  -  [VoiceMeeter Presets](#%EF%B8%8F-voicemeeter-presets)
  -  [Main Fader](#%EF%B8%8F-main-fader)
  -  [XTouch Display VU](#-x-touch-display--vu)
  -  [Transport Media Controls](#-transport--media-control)
  -  [Pedal Support](#%EF%B8%8F-pedal-support-xctrl-and-mackie-only)
  -  [XCTRL mode exclusives](#--)
- [Get Started](#%EF%B8%8F-get-started)
- [Requirements](#-requirements)
- [Future Expansion](#-future-expansion)
- [License](#-license)
- [Community](#-community)


## 🔩 X-Touch Modes
VM-XCtrl supports several X-Touch operating modes in LAN/USB/MIDI:
| Mode | Connection |
|---|---|
| **XCtrl** | LAN / MIDI |
| **XCtrl/Mackie** | LAN / MIDI |
| **XCtrl/HUI** | LAN / MIDI |
| **Mackie** | USB / MIDI |
>[!WARNING]
> **Some functionality is unavailable in XCtrl/Mackie and XCtrl/HUI modes due to hardware limitations**

> [!IMPORTANT]
> **Scribble Strips INVERTED colors aren't supported in Mackie mode**

---

## 🏷️ Features
VM-XCtrl is built around a multi-layer mixing workflow

<table width="100%" cellpadding="18">
  <tr>
    <td width="50%" valign="top">
    </br>
      <p align="center">
        <img src="https://img.shields.io/badge/INPUT-22C55E?style=for-the-badge&labelColor=172B3A">
      </p>
      <ul>
        <li>Mute, Solo, Volume and Mono controls</li>
        <li>Switch inputs to the Extension Inputs using the REC button</li>
        <li>Motorized faders with two-way feedback</li>
        <li>Input names and dynamic volume values on the X-Touch display</li>
        <li><strong>SELECT</strong> marks the input bus used by the SEND layer</li>
      </ul>
  </br>
    </td>
    <td width="50%" valign="top">
      </br>
      <p align="center">
        <img src="https://img.shields.io/badge/OUTPUT-38BDF8?style=for-the-badge&labelColor=172B3A">
      </p>
      <ul>
        <li>Mute, Solo, Volume and Mono controls</li>
        <li><strong>SELECT</strong> directly selects the VoiceMeeter bus through the VoiceMeeter API</li>
        <li>Select A1–B3 as the active destination for mixing</li>
        <li>Return to INPUT and build a custom mix for the selected bus</li>
        <li>Motorized faders and display feedback</li>
      </ul>
  </br>
    </td>
  </tr>
  <tr>
    <td width="50%" valign="top">
      </br>
      <p align="center">
        <img src="https://img.shields.io/badge/SEND-EF4444?style=for-the-badge&labelColor=172B3A">
      </p>
      <ul>
        <li>Assign input sends to VoiceMeeter outputs</li>
        <li>Adjust send amount directly with the fader</li>
        <li><strong>Main Fader</strong> can control all sends</li>
        <li><strong>FLIP</strong> switches between <strong>Absolute</strong> and <strong>Relative</strong> modes, matching native VoiceMeeter behavior</li>
      </ul>
  </br>
    </td>
    <td width="50%" valign="top">
      </br>
      <p align="center">
        <img src="https://img.shields.io/badge/APPS-FACC15?style=for-the-badge&labelColor=172B3A">
      </p>
      <ul>
        <li>Dedicated Windows Application Layer, independent from the VoiceMeeter API</li>
        <li>Dynamically detects active Windows applications</li>
        <li>Mute, Volume and percentage control</li>
        <li>Change Default output device or per application in real time</li>
        <li><strong>Instant</strong> or <strong>Confirm</strong> output device switching modes</li>
        <li>Short and full device names, with customizable short names for active or disconnected devices</li>
      </ul>
  </br>
    </td>
  </tr>
</table>

## ⚡ Additional Features

<table width="100%" cellpadding="18">
  <tr>
    <td width="100%" valign="top">

### 🗃️ VoiceMeeter Presets

- **F1–F8** recall VoiceMeeter presets directly from the X-Touch.

    </td>
  </tr>
  <tr>
    <td width="100%" valign="top">

### 🎚️ Main Fader

- The 9th / Main Fader can be reassigned in real time with `ALT + <Channel>` on all layers. On the SEND layer, it can control either the selected input send or the overall send level. It can also be disabled on the OUTPUT layer when not needed.

  </tr>
  <tr>
    <td width="100%" valign="top">

### 🎨 X-Touch Display & VU

- Customize screen colors for each VM-XCtrl layer.
- Display channel names and live volume values.
- Configurable VU meter response speed.
- Channels can be fully or partially disabled when the corresponding VoiceMeeter input or bus has no custom label, similar to VoiceMeeter Streamer View functionality.

    </td>
  </tr>
  <tr>
    
    <td width="100%" valign="top">
### 📻 Transport & Media Control

- The X-Touch transport controls provide Windows multimedia control:
  - **Previous · Next · Stop · Play**
- ❗ In **XCtrl/Mackie** and **XCtrl/HUI**, these controls are located in the **AUTOMATION** section
  - **Touch · Latch · Write · Read/Off**
>
  </tr>
  <tr>
    <td width="100%" valign="top">

### 🕹️ Pedal Support (XCtrl and Mackie only)
- VM-XCtrl supports all three X-Touch pedal inputs:
  - **2 × Footswitch**
  - **1 × Expression**
  
- Footswitches can mute any VoiceMeeter bus or duplicate any X-Touch button.
  The Expression pedal can control any bus volume or the Main Fader.
  An optional overlay can appear above all windows and show what the pedal is doing, for example when a microphone is muted or unmuted
  
  </tr>
  <tr>
    <td width="100%" valign="top">

### <p align="center"> <img src="https://img.shields.io/badge/XCtrl and Mackie-Exclusive%20ONLY-FF5A1F?style=for-the-badge&labelColor=172B3A"> </p>

- XCtrl mode provides additional functionality built specifically around the X-Touch hardware.
  - **TIMECODE** displays the current media position and active VM-XCtrl layer.
  - **JOG** wheel scrubs through music, video and audio by seconds.
  - Press **NUDGE** to make the JOG Wheel allow quick 5–10 second video jumps, similar to `J` / `K` in YouTube.
  - Multiple media capture modes are available, including classic Windows media targeting and **FOCUS** mode.
  - Pressing **SOLO** can force media control to the currently focused window.

    </td>
  </tr>
</table>

## ⚙️ Get Started
### Network-LAN connection
>[!TIP]
>* Connect the **X-Touch** to your local network using an Ethernet cable
>* Power it on while holding the **Select** button on **channel 1**
>* Choose mode **XCtrl** or **XCtrl/Mackie**
>   * _Note: Some features are not supported in XCtrl/Mackie mode — you can change this later in Settings_
>* In the **IFC** field, select **Network**
>* In the **Network** field, select **Slv IP**
>* Enter your computer **IP** address
>* Press **Select** to apply the settings
>* After a moment, the IP field on the X-Touch will show its address — enter that address in the field above
>   * _Note: It is recommended to reserve / assign a permanent IP for the X-Touch in your router (DHCP reservation), so the address does not change after the surface is powered off_
>* Select the same mode you set on the X-Touch for full compatibility
### USB/MIDI connection
>[!TIP]
>* Connect the **X-Touch** to your PC via USB cable or to your audio interface or related device via MIDI cable
>* Power it on while holding the **Select** button on **channel 1**
>* Choose mode **XCtrl** or **Mackie**
>* In the **IFC** field, select **USB** or **MIDI**
>* Press **Select** to apply the settings
>* After a moment, pick MIDI Input and MIDI Output devices (X-Touch by USB)
>* Select the same mode you set on the X-Touch for full compatibility

## 💎 Advantages

VM-XCtrl is designed as a preconfigured, ready-to-work application rather than a collection of manual mappings.

- Automatic connection and reconnection when VoiceMeeter or the X-Touch is restarted.
- Disconnect state (Issue) is reflected on the X-Touch.
- Windows autostart and automatic updates.
- Console and function customization.
- Left-clicking the tray icon provides VM-XCtrl status information.
- Support for future compatible VoiceMeeter releases.

## 🔐 Requirements

<p align="center">
  <img src="https://img.shields.io/badge/Windows-10%20%7C%2011-FF5A1F?style=for-the-badge&logo=windows&logoColor=white&labelColor=172B3A">
  <img src="https://img.shields.io/badge/VoiceMeeter-Potato%20%7C%20Banana-3D8BC9?style=for-the-badge&labelColor=172B3A">
  <img src="https://img.shields.io/badge/X--Touch-FULL-FF5A1F?style=for-the-badge&labelColor=172B3A">
  <img src="https://img.shields.io/badge/Connection-LAN%20%7C%20USB%20%7C%20MIDI-3D8BC9?style=for-the-badge&labelColor=172B3A">
</p>

>[!NOTE]
>- Windows 10 / 11
>- VoiceMeeter Potato 3.1.1.9+ / VoiceMeeter Banana 2.1.1.9+ or higher
>- Behringer X-Touch Full **(X-Touch Compact and Extender are not supported)**
>- LAN connection between the PC and X-Touch, or X-Touch connected to the PC over USB or MIDI

## 💫 Future Expansion
>[!WARNING]
>The current **VM-XCtrl Core** will continue to expand with additional functionality.
Larger future features may also be released as separate paid add-ons when they **EXTEND VM-XCtrl beyond direct VoiceMeeter** operation.

## 📋 License

VM-XCtrl is distributed under its own EULA.
You can evaluate the program during a 7-day free trial period.

[**EULA**](./docs/EULA.md) · [**Privacy Policy**](./docs/PRIVACY_POLICY.md) · [**Terms of Sale**](./docs/TERMS_OF_SALE.md)

<p align="center">
  <a href="https://vchaudio.gumroad.com/l/VM-XCtrl">
    <img src="https://img.shields.io/badge/Get%20a%20License-22C55E?style=for-the-badge&labelColor=172B3A">
  </a>
</p>


## 📌 Community

<p align="center">
  <a href="https://discord.gg/TxMyxPkBxw">
    <img src="https://img.shields.io/badge/Join%20the%20VM--XCtrl%20Discord-5865F2?style=for-the-badge&logo=discord&logoColor=white">
  </a>
</p>
