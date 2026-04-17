![VRC](Images/VRC.png)
> [!TIP]
> 💡 **Please leave all your feedback on the project's [Issues page](https://github.com/Kotin-ak/VRC-Releases/issues). It is critical for the app's growth and improvement. VRC is a free tool, and your input helps me make it better for everyone. If it works perfectly on your machine, please let me know! For bug reports and feature requests, use GitHub tickets.**

<div align="center">

# VRC (Video Recording Control Hub)

<a href="https://github.com/Kotin-ak/VRC-Releases/releases">
  <img src="https://img.shields.io/github/downloads/Kotin-ak/VRC-Releases/total?style=for-the-badge&color=2EA043&logo=github&logoColor=white" alt="Total Downloads" />
</a>
<a href="https://github.com/Kotin-ak/VRC-Releases/discussions">
  <img src="https://img.shields.io/badge/GitHub_Discussions-181717?style=for-the-badge&logo=github&logoColor=white" alt="Discussions" />
</a>
<a href="https://youtube.com/@vrc-hub">
  <img src="https://img.shields.io/badge/YouTube_Tutorials-FF0000?style=for-the-badge&logo=youtube&logoColor=white" alt="YouTube" />
</a>

<br />

###  📥 **[Download Latest Release](https://github.com/Kotin-ak/VRC-Releases/releases)**
###  🐛 [Report a Bug](https://github.com/Kotin-ak/VRC-Releases/issues)

</div>

### 🎬 Quick Demo

https://github.com/user-attachments/assets/7c67069e-30be-4646-a089-7777d7c0cc92

---

**VRC** is a centralized Windows application designed to remotely monitor and control multiple video production devices from a single dashboard. Stop jumping between different computers to manage your broadcast. With VRC, you have full remote command over your production nodes:

* 🔴 **Full Remote Control:** Launch, stop, and manage Recording, Streaming, External outputs, and Multicorder with a single click or customizable keyboard shortcuts (ideal for Elgato Stream Deck).
* 📊 **Deep Monitoring:** Track CPU/GPU performance and monitor available storage space in real-time via WMI to prevent recording failures.
* ⏰ **Smart Automation:** Built-in Task Scheduler to automate device commands based on precise timing.
* 🎛️ **Multi-Device Hub:** Support for **vMix** software mixers and **Blackmagic ATEM** hardware video switchers in a single workspace.

> **Supported Devices:**
> - **vMix** — deep integration via HTTP/TCP API (all editions).
> - **Blackmagic ATEM** — hardware video switcher control via COM SDK (requires Blackmagic ATEM Software Control installation).

<br />

### 🛠 Built With

<p>
  <img src="https://img.shields.io/badge/C%23_14-239120?style=for-the-badge&logo=c-sharp&logoColor=white" alt="C#" />
  <img src="https://img.shields.io/badge/.NET_10-512BD4?style=for-the-badge&logo=dotnet&logoColor=white" alt=".NET" />
  <img src="https://img.shields.io/badge/WinUI_3-0078D4?style=for-the-badge&logo=windows&logoColor=white" alt="WinUI 3" />
  <img src="https://img.shields.io/badge/XAML-0C54C2?style=for-the-badge&logo=xaml&logoColor=white" alt="XAML" />
</p>

---

## 📋 Table of Contents
> [!IMPORTANT]
> **New to VRC? Start with the [📥 Installation Guide](#installation) before anything else.**

- [Why VRC?](#why-vrc-the-problem-it-solves)
- [⚙️ System Requirements](#requirements)
- [**📥 Installation** *(start here!)*](#installation)
- [**🚀 Quick Start** *(5 minutes)*](#quickstart)
- [1. Dashboard](#1-dashboard) *(Basic)*
- [2. vMix Device Management](#2-vmix-device-management) *(Basic)*
- [3. Device Card](#3-device-card) *(Basic)*
  - [3.1. Header](#31-header)
  - [3.2. Status Indicators](#32-status-indicators)
  - [3.3. Program Monitor](#33-program-monitor)
  - [3.4. Inputs Tab](#34-inputs-tab--input-control)
  - [3.5. Audio Tab](#35-audio-tab--audio-mixer)
  - [3.6. List Tab](#36-list-tab--video-list-management)
  - [3.7. Outputs Tab](#37-outputs-tab--output-control)
  - [3.8. Replay Tab](#38-replay-tab--instant-replay)
  - [3.9. Scheduler Tab](#39-scheduler-tab--device-schedule)
  - [3.10. Card Footer](#310-card-footer)
- [4. PC Health Monitoring](#4-pc-health-monitoring) *(Optional · Advanced)*
- [5. Streaming Settings](#5-streaming-settings) *(Basic)*
- [6. Task Scheduler](#6-task-scheduler) *(Advanced)*
- [7. Shortcuts](#7-shortcuts-external-controller-integration) *(Advanced · Optional)*
- [8. Application Settings](#8-application-settings) *(Basic)*
  - [8.1. General](#general)
  - [8.2. Notifications](#notifications)
  - [8.3. Web Dashboard (settings)](#web-dashboard-settings)
  - [8.4. Control API](#control-api)
  - [8.5. Logs and Diagnostics](#logs-and-diagnostics)
  - [8.6. About](#about)
- [9. Web Dashboard](#9-web-dashboard) *(Optional)*
- [10. Navigation](#10-navigation) *(Basic)*
- **ATEM Support**
- [11. ATEM Device Management](#11-atem-device-management) *(Basic)*
- [12. ATEM Device Card](#12-atem-device-card) *(Basic)*
  - [12.1. Header](#121-header-1)
  - [12.2. Status Section](#122-status-section)
  - [12.3. Program Monitor](#123-program-monitor-1)
  - [12.4. Inputs Tab](#124-inputs-tab--input-control-1)
  - [12.5. Scheduler Tab](#125-scheduler-tab--device-schedule-1)
  - [12.6. Card Footer](#126-card-footer-1)
- [13. ATEM Command Catalog](#13-atem-command-catalog) *(Advanced)*
- **Watch Rules**
- [14. Watch Rules (Watchdog)](#14-watch-rules-watchdog) *(Advanced)*
  - [14.1. Rule Structure](#141-rule-structure)
  - [14.2. Triggers](#142-triggers)
  - [14.3. Conditions](#143-conditions)
  - [14.4. Actions](#144-actions)
  - [14.5. Cross-Device Monitoring](#145-cross-device-monitoring)
  - [14.6. Examples](#146-examples)
- **External Alerts**
- [15. External Alert Channels](#15-external-alert-channels) *(Advanced · Optional)*
  - [15.1. Supported Providers](#151-supported-providers)
  - [15.2. Device & Category Filters](#152-device--category-filters)
  - [15.3. Reliability: Retry & Circuit Breaker](#153-reliability-retry--circuit-breaker)
  - [15.4. Health Monitor](#154-health-monitor)
  - [15.5. Alert Delivery Log](#155-alert-delivery-log)
- [❓ FAQ & Troubleshooting](#faq)

---
## Why VRC? (The Problem It Solves)

In professional live production, you rarely rely on a single machine. You might have one vMix PC for the main mix, another for instant replays, and a third for graphics or encoding. Monitoring and controlling all of them simultaneously usually requires a large crew or constantly switching between KVMs, which leads to missed cues, high stress, and potential on-air failures.

VRC was built to solve this exact problem. It turns any Windows tablet or laptop on your network into a **Master Control Room**.

### Who is this for?
* **Solo Operators & Small Crews:** Manage recording, streaming, and switching across multiple PCs without needing extra hands. Ideal for local sports, corporate events, and live gigs.
* **Esports Productions:** Control complex multi-node setups (player POVs, caster desks, main feed) from one central hub with precision timing.
* **Broadcast Engineers & Technical Directors:** Monitor CPU and GPU loads, audio levels, and crucially, **track remaining free disk space** across all nodes in real-time. Prevent stream crashes and ruined recordings before they happen.

---

<a id="requirements"></a>
## ⚙️ System Requirements

| Component | Requirement |
|-----------|-------------|
| **OS** | Windows 10 (build 19041+) or Windows 11 |
| **Architecture** | x64 only |
| **Runtime** | Windows App Runtime 2.0 *(bundled in the release package)* |
| **vMix** | Any version · v29+ recommended for full feature support (GO button) |
| **ATEM** | *(Optional)* **Blackmagic ATEM Software Control** must be installed on the VRC machine (provides the COM SDK). Any ATEM model supported |
| **Network** | LAN access to devices. vMix: HTTP `8088`, TCP `8099`. ATEM: UDP `9910` (proprietary Blackmagic protocol) |
| **WMI Monitoring** | *(Optional)* Windows credentials on each remote machine — see [Section 4](#4-pc-health-monitoring) |

---

<a id="installation"></a>
## 🛠 Installation (Important!)

> [!IMPORTANT]
> Because VRC is a locally signed .msix package, you **MUST** install the security certificate first, otherwise Windows will block the installation.

1. Download the `.zip` archive from the Releases page and extract it.
2. **Install the security certificate:** Right-click the certificate file, select Install, and place it in **"Local Machine" -> "Trusted People"**.
3. **Install Dependencies:** The extracted folder contains a `Dependencies` directory with additional required resources. Since this is a 64-bit Windows package, navigate to `Dependencies\x64` and install the Windows App Runtime by double-clicking: `Microsoft.WindowsAppRuntime.2.0-preview1.msix`
4. **Install VRC:** Finally, double-click the main VRC `.msix` file to install the app.

---

<a id="quickstart"></a>
## 🚀 Quick Start (First 5 Minutes)

> [!TIP]
> **Already installed?** Follow these steps to get up and running immediately.

1. **Launch VRC** — you'll see an empty Dashboard.
2. Click **Add vMix** (`Ctrl+N`), enter your vMix machine's IP address and port, then click **Probe** to verify the connection.
3. Click **Save** — the device card appears on the Dashboard.
4. Wait for the connection indicator in the card header to turn **green** *(connected)*.
5. Click the **🔒 Lock icon** in the card footer to unlock controls — all buttons are locked by default to prevent accidental actions on air.

> ✅ **Done.** Click any status indicator — **REC**, **STREAM**, **EXT** — to control your vMix remotely.

---

## 1. Dashboard

The main screen of the application — a grid of connected device cards with real-time monitoring.

> [!TIP]
> **Controls not responding?** Each card has a **🔒 Lock** in its footer — active by default. Click it to unlock the card and enable all control buttons. See [3.10. Card Footer](#310-card-footer).

---


![Dashboard](Images/Win11.4K.png)

### Command Bar (Workspace Management)

**What are Presets and Configurations?**
* **Preset:** A saved group of vMix machines (your specific workspace). If you travel between different venues, you can save a preset for "Studio A" and another for "Away Tournament". Load a preset, and VRC instantly connects to the exact vMix nodes for that location without requiring you to re-enter IP addresses manually.
* **Configuration:** A master backup of your VRC application, including *all* your presets and global settings. Use this to quickly clone your entire VRC setup to a secondary or backup control laptop.

| Action | Shortcut | Business Value / Description |
|--------|----------|------------------------------|
| **Add vMix** | `Ctrl+N` | Connect a new vMix node to your current workspace |
| **Add ATEM** | — | Connect a new Blackmagic ATEM video switcher to your workspace |
| **Last Session** | — | Quickly restore the exact machines you were monitoring when you last closed VRC |
| **Save Preset** | `Ctrl+S` | Save your current grid of vMix machines to load them instantly next time |
| **Card Size** | — | Adjust how much screen space each device card takes |

The status bar displays the current preset name and the number of connected devices.

#### Additional Commands (overflow menu "⋯")

| Action | Shortcut | Business Value / Description |
|--------|----------|------------------------------|
| **Save As…** | `Ctrl+Shift+S` | Duplicate your current workspace under a new name (e.g., "Tournament Day 2") |
| **Delete Preset** | — | Remove a workspace setup you no longer need |
| **Export Preset** | — | Save a specific workspace layout to a file to share with another operator |
| **Import Preset** | — | Load a workspace layout provided by someone else |
| **Export Configuration** | — | Create a master backup of your entire VRC setup to easily migrate to another PC |
| **Import Configuration** | — | Restore your master backup on a new control laptop |


### Card Display

- Device cards are arranged in an adaptive grid that automatically adjusts to the window size.
- **Pagination** — when there are many devices, cards are split across pages with a dot indicator for navigation. Mouse wheel scrolling is supported.

---

## 2. vMix Device Management

### Adding a Device

![Add vMix dialog](Images/AddvMix.png)

When adding a new vMix device, the following fields are specified:

- **Name** — custom name (up to 20 characters).
- **IP Address** — address of the machine running vMix.
- **HTTP Port** — vMix Web API port.
- **TCP Port** — TCP API port (configured automatically).
- **Polling Interval** — data refresh rate (250–5000 ms).
- **Login and Password** — credentials for authorization (if required).
- **Transport Mode** — communication method with vMix (HTTP, TCP, etc.). A warning about limitations is displayed when HTTP is selected.
- **Time Zone** — time zone assignment for the device to ensure correct time display during remote operation.

### Connectivity Check (Probe)

Before saving, you can test the connection to the device. The result and details are displayed directly in the dialog.

### Connection Options

- **Auto-Connect** — automatically connect to the device on application startup.
- **Auto-Reconnect** — automatically restore the connection when it is lost.

### Device Actions

Available through the card context menu:

- **Streaming Settings** — open the streaming channel management dialog.
- **Edit** — modify connection parameters.
- **WMI Settings** — configure remote PC monitoring.
- **Logs** — view the device event log.
- **Delete** — remove the device from the configuration.
- **Move to…** — move the device between groups.

---

## 3. Device Card

Each connected vMix device is displayed as a card with full real-time information. 

> [!NOTE]
> **Safety First:** By default, all control actions on the card are **LOCKED** to prevent accidental clicks during a live broadcast. To enable control, you must first click the **Lock (🔒)** icon in the card footer.

### 3.1. Header

- Device name, IP address, transport mode.
- vMix version and edition, preset name.
- Device time zone.
- Color-coded connection status indicator.
- **Context menu (⋯)** — streaming settings, edit, WMI, logs, delete, move between groups.

### 3.2. Status Indicators

![Status indicators](Images/StatusSection.png)

> [!NOTE]
> Some indicators (**Multicorder**, **Replay**, extended **Overlay** layers, additional **Output** channels) are only visible if your vMix edition and version support them. The **GO** button requires vMix v29+; earlier versions show **QuickPlay** instead.

Interactive indicators — clicking toggles the corresponding vMix function:

| Indicator | Click | Details |
|-----------|-------|---------|
| **Streaming** | Start/stop all channels | Individual channel indicators 1–5 (each clickable). Number of channels depends on vMix edition |
| **Recording** | Start/stop recording | Primary and secondary recorder indicators, recording duration timer |
| **Multicorder** | Start/stop multi-recording | Displayed only when supported by the vMix edition |
| **Replay** | Start/stop Instant Replay recording | Displayed only when supported by the vMix edition |
| **External** | Toggle external output on/off | Tooltip with output configuration details |
| **Fullscreen** | Toggle fullscreen mode on/off | Tooltip with current settings |
| **Playlist** | Start/stop playlist | — |
| **Overlay** | Disable all overlays | Individual indicators per layer (each clickable separately) |

### 3.3. Program Monitor

![Program monitor](Images/ProgramMonitor.png)

Section displaying the current source in Program/Preview with audio levels.

#### Monitor Source Selection

Via the dropdown menu or by scrolling the mouse wheel:

| Source | Description |
|--------|-------------|
| **Program** | Main program output |
| **Preview** | Preview output |
| **PRV\|PGM** | Automatic — displays the active source |
| **Output 1–4** | External outputs (Output 3–4 when supported) |
| **Overlay 1–8** | Overlay layers (Overlay 5–8 with extended overlays) |

#### Information Panel

- **Current input name** — name and label of the playing source.
- **Progress bar** — for playable sources (video), showing remaining time.
- **Playback status** — Play / Pause / Stop icons.
- **Loop** — loop indicator.
- **List position** — element index display for video lists.
- **Title text** — current text for title inputs.

#### Master Audio Meter

- Dual-channel (L/R) vertical Master bus level indicator.
- Gradient: green (normal) → yellow (headroom) → red (clipping).
- Tooltip with peak values (dBFS).

### 3.4. Inputs Tab — Input Control

![Input control section](Images/InputsSection.png)

List of all vMix inputs with pagination.

#### Available for each input:

**Primary actions (buttons):**

| Action | Description |
|--------|-------------|
| **GO / QuickPlay** | Transition to input (GO for vMix v29+, QuickPlay for earlier versions) |
| **Cut** | Instant switch to input via Cut |
| **Play / Pause** | Play / pause (for video inputs) |
| **Loop** | Toggle playback looping on/off |
| **Mute** | Mute / unmute input audio |

**Input overlays (4×2 grid):**

- Toggle overlay layers 1–8 individually by clicking.
- Overlay context menu for additional actions.

**Input context menu (right-click):**

| Action | Description |
|--------|-------------|
| **Active** | Send input to Program |
| **Preview** | Send input to Preview |
| **Restart** | Restart playback (for video) |
| **AutoPause** (On/Off) | Auto-pause when switching away from the input |
| **AutoPlay** (On/Off) | Auto-play when switching to the input |
| **AutoRestart** (On/Off) | Auto-restart on completion |
| **Video Source** (1–4) | Select video source for Video Call inputs |
| **Audio Source** | Select audio source for Video Call: Master, Headphones, Bus A–G |

**Indicators:**

- Audio levels (dual-channel L/R meter) for each input.
- Color-coded border: green (Preview) / red (Program).
- Input type icon (camera, video, titles, etc.).

### 3.5. Audio Tab — Audio Mixer

Full-featured audio mixer with separate control of the master bus, buses, and inputs.

#### Master Bus

| Action | Description |
|--------|-------------|
| **Mute** | Mute / unmute Master |
| **Volume slider** | Master level adjustment (0–100%) via popup fader |
| **Audio meter** | Dual-channel L/R level indicator |

![Audio mixer — buses](Images/AudioOutputsSection.png)

#### Audio Buses (Bus A–G)

For each available bus:

| Action | Description |
|--------|-------------|
| **Mute** | Mute / unmute bus |
| **Send to Master (M)** | Route bus to master |
| **Volume slider** | Bus level adjustment (0–100%) |
| **Solo (S)** | Solo-listen the bus |
| **Audio meter** | Dual-channel L/R level indicator |

#### Per-Input Audio

![Audio mixer — inputs](Images/AudioInputsSection.png)

For each input with audio:

| Action | Description |
|--------|-------------|
| **Mute** | Mute / unmute input audio |
| **AFV** | Audio Follow Video — automatic audio control on switching |
| **Routing (M, A–G)** | Assign input to buses: Master and Bus A–G (individually, by click) |
| **Volume slider** | Input level adjustment (0–100%) via popup fader |
| **Solo (S)** | Solo-listen the input |
| **Audio meter** | Dual-channel L/R level indicator |

### 3.6. List Tab — Video List Management

![Video list section](Images/ListSection.png)

Video list (playlist) management for vMix. Displayed when video lists are present.

#### Information Panel

- Current list name and its state (Playing / Paused / Stopped).
- Position / duration / remaining time.
- Number of items in the list.
- Playback progress bar.

#### Item List

- Display of all files in the list with duration.
- Color highlight for the currently playing item.
- Enabled/disabled item indicator.
- **Context menu**: Select, Remove (remove from list).

#### Playback Controls

| Button | Description |
|--------|-------------|
| **⏮ Previous** | Previous list item |
| **⏯ Play / Pause** | Play / pause |
| **⏭ Next** | Next list item |
| **🔀 Shuffle** | Shuffle the list |
| **🔁 Loop** | Loop the list |

#### Additional Commands (overflow menu "⋯")

| Command | Description |
|---------|-------------|
| **Play Out** | Play with automatic completion |
| **Auto Next** | Auto-advance to the next item |
| **Auto First** | Auto-return to the first item |

#### List Navigation

- Switch between multiple video lists via the dot indicator (PipsPager).

### 3.7. Outputs Tab — Output Control

![Outputs section](Images/OtputsSection.png)

Detailed display and control of vMix outputs.

#### Fullscreen Outputs

| Output | Description |
|--------|-------------|
| **Fullscreen 1** | Primary fullscreen output — source selection via SplitButton |
| **Fullscreen 2** | Secondary fullscreen output (when dual-monitor support is available) |

#### External Outputs (Output 1–4)

For each output, the following is displayed:

- **Source** — currently assigned source (changeable for Output 2–4).
- **NDI** — NDI streaming status (On/Off).
- **OMT** — OMT output status (On/Off).
- **SRT** — SRT streaming status (clickable to toggle).

> Output 3 and Output 4 are displayed only for vMix editions with four external outputs.

### 3.8. Replay Tab — Instant Replay

Section for Instant Replay control (implementation in progress).

### 3.9. Scheduler Tab — Device Schedule

![Scheduler section on card](Images/SchedulerSection.png)

Compact list of scheduled tasks for the given device.

- Display of upcoming tasks: time, function, parameters, status.
- Time-until-next-task indicator.
- **Open Scheduler** button — navigate to the full scheduler page.

### 3.10. Card Footer

| Element | Description |
|---------|-------------|
| **🔒 Lock** | Lock	Default state: ON. Protects against accidental actions. When active, all control buttons are locked. Click to toggle. |
| **🔽 Collapse Audio** | Show/hide the audio section (with icon rotation animation) |
| **🔔 Notifications** | Enable/disable notifications for a specific device (green — on, gray — off) |
| **⚠ Errors** | Display of current connection errors (in red) |
| **⏳ Spinner** | Loading indicator while an operation is in progress |
| **🔘 Connection Toggle** | Enable/disable connection to the device |

---

## 4. PC Health Monitoring

![PC monitoring](Images/PCMonitoringSection.png)

### PC Health Monitoring (WMI)

Remote collection of workstation metrics for the machine running vMix:
* CPU — processor load (with critical value highlighting).
* GPU 3D & Encode — graphics card and hardware video encoder load.
* Disks — free space monitoring.

Data is collected natively via Windows Management Instrumentation (WMI).

#### 🛠 Seamless WMI Configuration
Configuring WMI across a network usually involves tedious firewall and UAC tweaking. To make this painless, the VRC settings menu provides built-in PowerShell scripts to automate the setup:

1. Remote PC (Target vMix Machine): Click Copy -> Remote PC in VRC and run the script in PowerShell (as Administrator) on the target machine. This automatically configures WMI permissions, Windows Firewall, and UAC (LocalAccountTokenFilterPolicy) for remote access.
2. This PC (VRC Host): Click Copy -> This PC and run it locally to add the remote machine to your TrustedHosts list.
3. Credentials: Enter the Windows login and password of the remote PC.
   * *Workgroup:* Just use the username.
   * *Domain:* Use DOMAIN\username or .\username for local admin.
4. Network Ports: If you are monitoring across different subnets, ensure your corporate routers allow traffic over TCP port 135 and the dynamic RPC range (49152–65535).

![WMI monitoring settings](Images/PCMonitoringsSettings.png)

---

## 5. Streaming Settings

![Streaming settings](Images/StreamingSettingsvMix.png)

A dedicated dialog for managing streaming channels of a specific device:

- Individual toggles (Start/Stop) for each channel.
- Connection status and vMix version display.
- Edition and IP address information.

---

## 6. Task Scheduler

Centralized management of deferred and recurring commands for all devices.

### Task Creation

- **Name** — custom task name.
- **Device** — target device selection.
- **Category and Function** — command selection from a hierarchical catalog.
- **Parameters** — additional command parameters (dynamically dependent on the selected function).
- **Schedule** — type: one-time / daily / weekly.
- **Time and Date** — exact execution moment (24-hour format).
- **Retries** — number of retry attempts on failure (1–10).
- **Enable/Disable** — individually per task.

### Task Management

- **Global toggle** — enable/disable the entire scheduler.
- **Filtering** — by device and by status.
- **Tabs**: all tasks, upcoming (24 h), errors.

### Bulk Actions

| Action | Description |
|--------|-------------|
| **Hold** | Suspend selected tasks |
| **Run Now** | Immediately execute selected tasks |
| **+5 / +10 / +15 min** | Postpone execution by the specified time |
| **Cancel** | Cancel selected tasks |
| **Restore** | Restore canceled tasks |

### Additional Details

![Scheduler — task list](Images/SchedulerPage.png)

- Indication of disconnected devices in the task list.
- Warning banner when the scheduler is disabled.
- Last execution result display in the details panel.

---

## 7. Shortcuts (External Controller Integration)

![Shortcuts page](Images/Shortcuts.png)

Binding external controller buttons (Stream Deck, Companion, Touch Portal, etc.) to VRC device commands. All configuration is done entirely within VRC — the external device acts as a "thin client" that only reports button presses.

> The approach mirrors the vMix Shortcuts model: no configuration is needed on the controller side.

### How It Works

![Stream Deck integration](Images/StreamDeck.jpg)

1. The user drags a "VRC Control" action onto a Stream Deck button — **done**. No additional setup is required on the controller side.
2. The button automatically receives a unique ID (the action UUID from the Stream Deck SDK).
3. The plugin connects to VRC's local Control API (`localhost:5101`) via SignalR.
4. In VRC, the user opens **Shortcuts** and creates a new shortcut by clicking **Add**.
5. The **Find Control** dialog opens — the user presses a physical button on the controller.
6. VRC captures the button ID and creates a `ShortcutEntry` linked to that key.
7. The user configures the command: **Device → Category → Function → Parameters**.
8. When the button is pressed during operation, VRC looks up the shortcut by key and executes the bound command on the target device.

### Page Layout

![Shortcuts demo](Images/ShortcutsDemo.png)

Master-detail layout (similar to the Scheduler page).

#### Command Bar

| Action | Description |
|--------|-------------|
| **Add** | Create a new shortcut (opens the detail panel in creation mode) |

#### Master Panel (Left — Shortcut List)

- **Device filter** — filter shortcuts by target device (ComboBox with an "All devices" option).
- Table columns: checkbox (enabled/disabled), status indicator, Key, Device, Function, Title.
- Row selection highlights the item and loads it into the detail panel.
- Clicking an empty area deselects the current shortcut.
- **Reorder arrows** (▲ / ▼) — move the selected shortcut up or down in the list.

#### Detail Panel (Right — Shortcut Editor)

When no shortcut is selected, an empty state is displayed with a prompt to select or create a shortcut.

When a shortcut is selected or being created:

| Field | Description |
|-------|-------------|
| **Key** | External button identifier (read-only, set via Find Control) |
| **Find Control** | Opens the button detection dialog |
| **Title** | Human-readable name for the shortcut |
| **Device** | Target device for command execution |
| **Category** | Command category from the hierarchical catalog |
| **Function** | Specific function within the category |
| **Parameters** | Dynamic parameters dependent on the selected function |
| **Enabled** | Toggle switch to enable/disable the shortcut |

#### Feedback Settings

Configures visual feedback sent back to the external controller button.

| Field | Description |
|-------|-------------|
| **Event** | ACTS event type for feedback (e.g., Recording, Streaming, Input, Overlay, etc.) |
| **Input Number** | Input number for input-bound events (shown only for relevant event types) |
| **Color** | Feedback color for the button when the event is active (8 preset colors with a palette picker) |

Available feedback events:

**vMix devices:**

| Category | Events |
|----------|--------|
| **Global** | Recording, Streaming, External, Fullscreen, FadeToBlack, MasterAudio, Bus A–G Audio |
| **Input-bound** | Input (Program), InputPreview, InputPlaying, InputAudio, InputSolo, InputLoop, Input Bus routing (A–G, Master), InputAudioAuto |
| **Overlays** | Overlay 1–8 |

**ATEM devices:**

| Category | Events |
|----------|--------|
| **Global** | Streaming, Recording, FadeToBlack, Transition, DSKOnAir |
| **Input-bound** | InputProgram, InputPreview |
| **HyperDeck** | HyperDeckRecord, HyperDeckPlay |

#### Action Buttons

| Button | Description |
|--------|-------------|
| **Save** | Save the shortcut configuration |
| **Cancel** | Cancel creation (visible only in creation mode) |
| **Delete** | Delete the selected shortcut |

### Find Control Dialog

A modal dialog for detecting external controller buttons:

1. Displays a progress ring and a prompt: "Press a button on your controller…"
2. When a button press is received via SignalR (`IdentifyButton`), the dialog shows the captured button ID.
3. The user confirms with OK — the key is assigned to the shortcut.

> The `IdentifyButton` method is separate from `execute` — pressing a button during detection does **not** trigger the bound command.

### Shortcut Execution Flow

1. External device sends `POST /api/shortcuts/execute { "buttonId": "uuid" }` to `localhost:5101`.
2. VRC: `ShortcutExecutor.ExecuteByKeyAsync(buttonId)` → `ShortcutStore.FindByKey` → check `IsEnabled` → `DeviceManager.GetDeviceById` → `DeviceClient.SendAsync(DeviceCommand)`.
3. If feedback is configured, VRC sends the current state back to the controller via SignalR.

---

## 8. Application Settings

### General

![Settings — general](Images/SettingsAplication.png)

| Parameter | Description |
|-----------|-------------|
| **Language** | Interface language selection (Russian / English) |
| **Minimize to Tray** | Application minimizes to the system tray instead of the taskbar |
| **Auto-Start** | Auto-launch the application on Windows login |
| **Multiple Instances** | Allow running multiple copies of the application |

### Notifications

| Parameter | Description |
|-----------|-------------|
| **Notifications** | Enable/disable Windows Toast notifications |
| **Mode** | All / Critical / Broadcast / Off |
| **Connection Notifications** | Alerts on device connect/disconnect |
| **Silent Mode** | Suppress notification sounds |
| **External Alert Channels** | Configure Telegram, Discord, Slack, Teams, and other external providers — see [Section 15](#15-external-alert-channels) |

### Web Dashboard

![Settings — web dashboard](Images/SettingsWebDashboard.png)

| Parameter | Description |
|-----------|-------------|
| **Enable** | Activate the built-in web server |
| **Port** | Port configuration (1–65535) |
| **Local URL** | Link to the dashboard for this PC |
| **LAN Addresses** | List of addresses for LAN access |

### Control API

| Parameter | Description |
|-----------|-------------|
| **Enable** | Activate the built-in HTTP Control API server |
| **Port** | Port for the API server (1–65535); default `5101` |
| **API Key** | Authentication key for HTTP requests — use **Generate** to create a random key, **Copy** to copy it to clipboard |
| **Status** | Whether the API key is currently configured |
| **Documentation** | Link to the full API reference |
| **Stream Deck Plugin** | Install the VRC Control action plugin for Elgato Stream Deck |

> When an API Key is configured, all HTTP requests must include the `X-Api-Key: {key}` header.

#### HTTP Endpoints

| Method | Endpoint | Body | Description |
|--------|----------|------|-------------|
| `GET` | `/api/status` | — | VRC server status, version, device count, and device list |
| `GET` | `/api/devices` | — | List of all registered devices |
| `GET` | `/api/devices/{id}` | — | Device info by ID |
| `POST` | `/api/devices/{id}/command` | `ApiCommandRequest` | Execute a named command on the specified device |
| `GET` | `/api/devices/{id}/commands` | — | Available commands for the device (grouped by category) |
| `GET` | `/api/devices/{id}/commands/{category}/{function}/parameters` | — | Parameters for a specific function |
| `POST` | `/api/shortcuts/execute` | `ApiShortcutExecuteRequest` | Execute a shortcut by external button ID |

> **Audit logging:** `POST /api/shortcuts/execute` writes `CMD [External]` to the device audit log. `POST /api/devices/{id}/command` writes `CMD [API]` to the device audit log.

**`GET /api/status` — response:**
```json
{
  "isRunning": true,
  "deviceCount": 2,
  "version": "1.5.0",
  "devices": [
    { "id": "...", "name": "Studio A", "type": "vMix", "ipAddress": "192.168.1.10", "isConnected": true }
  ]
}
```

**`POST /api/devices/{id}/command` — request body:**
```json
{ "deviceId": "...", "commandName": "StartRecording", "parameters": null }
```

**`POST /api/shortcuts/execute` — request body:**
```json
{ "buttonId": "uuid-of-stream-deck-action" }
```

#### SignalR Hub (`/hubs/control`)

| Direction | Method | Payload | Description |
|-----------|--------|---------|-------------|
| Server → Client | `ButtonFeedback` | `ApiButtonFeedback` | Button state update sent back to the external controller |
| Server → Client | `ActivatorEvent` | `ApiActivatorEvent` | Real-time ACTS event broadcast (tally, audio levels, recording status) |
| Client → Server | `IdentifyButton` | `buttonId` | Button identification request during shortcut setup |

**`ButtonFeedback` payload:**
```json
{ "buttonKey": "91AC8", "isOn": true, "eventType": "Recording", "color": "#E53935" }
```

**`ActivatorEvent` payload:**
```json
{ "deviceId": "...", "eventType": "Input", "inputNumber": 3, "value": 1.0, "isOn": true }
```

### Logs and Diagnostics

![Settings — logs and diagnostics](Images/SettingsLogs.png)

| Parameter | Description |
|-----------|-------------|
| **Device Logs** | Open the device log folder |
| **GC Monitor** | Garbage collector monitoring status and logs |

#### Log File Structure

All log files are stored in the app's local data folder and are accessible via the **Device Logs** button.

| File | Retention | Contents |
|------|-----------|----------|
| `{DeviceName}_{id}/audit-YYYYMMDD.log` | 30 days | Per-device audit: connections, state changes, ACTS events, operator commands |
| `Alerts/alerts-YYYYMMDD.log` | 30 days | External alert delivery: sent, failed (with retry attempts), circuit breaker open/close events |
| `Updates/update-YYYYMMDD.log` | 90 days | Update history: check, download, install, errors with HRESULT codes |
| `_system/gc-health-YYYYMMDD.log` | 30 days | .NET memory metrics: heap, working set, GC generation counters, fragmentation |
| `_system/hw-monitor-YYYYMMDD.log` | 30 days | Hardware threshold events: CPU/GPU/disk alerts and recoveries |

#### Per-device audit log (`audit-*.log`)

| Event | Example entry |
|-------|---------------|
| **Connection** | `Connected (192.168.1.10:8099, Tcp)` |
| **Reconnect / error** | `Reconnect (Reconnecting/Network): Host unreachable` |
| **Disconnection** | `Disconnected (UserRequested)` |
| **Initial snapshot** | `Snapshot Rec=False Stream=False Ext=False MC=False FS=False` |
| **Lock / Unlock** | `🔓 Unlocked (Lock)` / `🔒 Locked (Lock)` |
| **State change** | `Δ Recording: false → true Rec=—` |
| **State change** | `Δ Streaming: true → false Rec=00:15:42` |
| **ACTS event** | `ACTS Recording Value=1 Rec=00:15:42` |
| **ACTS event** | `ACTS Overlay2 Input=13 Value=1 Rec=—` |
| **UI button (intent)** | `CMD [Operator] Send: StartStopRecording Rec=—` |
| **UI button (success)** | `CMD [Operator] Send: StartStopRecording -> OK` |
| **UI button (error)** | `CMD [Operator] Send: StartStopStreaming -> ERROR: timeout` |
| **Scheduler (success)** | `CMD [Timer] Send: StartRecording -> OK 'Morning Rec' (attempt 1/3)` |
| **Scheduler (error)** | `CMD [Timer] Send: StartRecording -> ERROR: not connected 'Morning Rec' (attempt 2/3)` |
| **Shortcut (success)** | `CMD [External] Send: StartRecording -> OK 'REC Button'` |
| **Shortcut (error)** | `CMD [External] Send: StartRecording -> ERROR: timeout 'REC Button'` |

#### Hardware threshold log (`_system/hw-monitor-*.log`)

Writes only on threshold crossings — not on every poll cycle.

| Threshold | Trigger condition |
|-----------|-------------------|
| **CPU** | Usage > 90% (crossed / recovered) |
| **GPU** | Encode usage > 95% (crossed / recovered) |
| **Disk** | Free < 10 GB or free < 10% (crossed / recovered) |

Example entries:

```
WRN [192.168.1.10] CPU load crossed threshold: 92.3% (threshold 90%)
INF [192.168.1.10] CPU load recovered: 74.5%
WRN [192.168.1.10] GPU Encode load crossed threshold: 96.0% (threshold 95%)
WRN [192.168.1.10] Disk C: free space dropped below threshold — 8.5 GB (6.2% free)
INF [192.168.1.10] Disk C: free space recovered — 15.2 GB (11.4% free)
```

### About

![Settings — about](Images/SettingsAboutTheProgram.png)

| Parameter | Description |
|-----------|-------------|
| **Version** | Current application version |
| **Updates** | Check, download, and install updates with progress |
| **Release Notes** | Link to the release page |
| **Reset Settings** | Restore all settings to defaults |

### ⌨️ Keyboard Shortcuts Reference

| Shortcut | Action |
|----------|--------|
| `Ctrl+N` | Add a new vMix device |
| `Ctrl+S` | Save current preset |
| `Ctrl+Shift+S` | Save preset under a new name (Save As…) |

---

## 9. Web Dashboard

![Web dashboard — interface](Images/WebDashboard.png)

Built-in read-only dashboard accessible from any browser on the local network.

- **Real-time updates** via SignalR with automatic reconnection.
- Display of all connected devices with indicators:
  - **REC** — recording.
  - **STREAM** — streaming.
  - **EXT** — external output.
  - **MCR** — multicorder.
  - **FS** — fullscreen mode.
  - **FTB** — Fade to Black.
- **Audio meters** — audio level visualization.
- LAN access via a configurable port.

---

## 10. Navigation

- Left sidebar with a tree structure of devices (groups and subgroups).
- Quick access to **Settings** via the built-in navigation button.
- Dedicated **Scheduler** page for global management of all tasks.
- Dedicated **Shortcuts** page for external controller button bindings.
- Page caching — state is preserved when switching between sections.

---

## 11. ATEM Device Management

> [!NOTE]
> ATEM support requires **Blackmagic ATEM Software Control** to be installed on the VRC machine. The application provides COM SDK components that VRC uses to communicate with ATEM switchers. If the software is not installed, VRC will display a clear error message when attempting to connect.

### Adding an ATEM Device

Click **Add ATEM** on the Dashboard command bar to open the ATEM device addition dialog.

| Field | Description |
|-------|-------------|
| **Name** | Custom device name (up to 20 characters) |
| **IP Address** | IP address of the ATEM video switcher (default: `192.168.10.240`) |

### Connectivity Check (Probe)

Before saving, you can verify network reachability using the **Probe** button. Unlike vMix (which tests a TCP connection), the ATEM probe uses **ICMP ping**, since ATEM communicates over UDP and has no TCP listener.

### Connection Options

| Parameter | Description |
|-----------|-------------|
| **Auto-Connect** | Automatically connect to the switcher on application startup |
| **Auto-Reconnect** | Automatically restore the connection when it is lost |

### Connection Protocol

VRC communicates with ATEM video switchers via the **Blackmagic COM SDK** on a dedicated STA thread (Single-Threaded Apartment). The protocol uses **UDP port 9910** (proprietary Blackmagic protocol). Connection is established with a 15-second timeout; disconnection — with a 5-second timeout.

### Auto-Detection of Model

Upon connection, VRC automatically reads the product name of the switcher (e.g., "ATEM Mini Extreme ISO", "ATEM Television Studio HD8 ISO") and displays it in the card header next to the device name.

### Device Actions

Available through the card context menu:

- **Edit** — modify connection parameters (IP address, name).
- **Logs** — view the device audit log.
- **Delete** — remove the device from the configuration.
- **Move to…** — move the device between groups.

### Error Handling

VRC provides clear localized error messages for common ATEM connection issues:

| Condition | Error Message |
|-----------|---------------|
| **ATEM Software Control not installed** | Prompts the user to install the software (COM components missing) |
| **Switcher not responding** | The ATEM switcher at the specified IP did not respond |
| **Incompatible firmware** | The switcher firmware is incompatible with the installed SDK version |
| **Connection timeout** | Connection timeout exceeded |
| **COM error** | General COM interaction error with HRESULT details |

---

## 12. ATEM Device Card

Each connected ATEM video switcher is displayed as a card with real-time status information and control, following the same card paradigm as vMix devices.

> [!NOTE]
> **Safety First:** As with vMix cards, all control actions are **LOCKED** by default. Click the **Lock (🔒)** icon in the card footer to unlock the card before sending commands.

### 12.1. Header

- Device name and IP address.
- **Product name** — automatically detected switcher model (e.g., "ATEM Mini Extreme ISO").
- Blackmagic brand indicator.
- Color-coded connection status indicator (green = connected, gray = disconnected, animated = reconnecting).
- **Context menu (⋯)** — edit, logs, delete, move between groups.

### 12.2. Status Section

The ATEM status section is a composite panel of up to 8 independent indicators. Each indicator is displayed only when the corresponding feature is available on the connected switcher model.

> [!NOTE]
> Feature availability depends on the ATEM switcher model and firmware. For example, Streaming and USB Recording are available only on models with a built-in encoder (ATEM Mini series). HyperDeck indicators appear only when HyperDecks are connected. Camera Recording requires Blackmagic cameras connected via SDI.

Interactive indicators — clicking toggles the corresponding function:

| Indicator | Click | Details |
|-----------|-------|---------|
| **Streaming** | Start/stop RTMP/SRT streaming | Duration timer, connection status. Available on ATEM Mini series and models with built-in encoder |
| **Recording** | Start/stop USB recording | Per-disk indicators (Disk 1 / Disk 2). Duration timer. **Switch Disk** action available |
| **HyperDeck** | Start/stop recording on all connected HyperDecks | Per-deck indicators (each clickable: Record / Stop / Play). Bulk actions Record All / Stop All |
| **Camera Rec** | Start/stop recording on Blackmagic cameras via SDI | Per-camera indicators. Bulk actions Start All / Stop All. Uses SDI Camera Control Protocol v1.6.2 (VANC, embedded in SDI signal) |
| **DSK** | Toggle Downstream Keyer on air | Per-key indicators (DSK 1, DSK 2, etc.). Each key toggleable individually. Auto-transition support |
| **FTB** | Trigger Fade to Black | Per-M/E indicators. Rate and FullyBlack control |
| **M/E** | Trigger transition (Cut / Auto) | Per-M/E block indicators. Program/Preview input display. Transition position control |
| **Info** | — (read-only) | Current video mode (e.g., 1080p50, 2160p30). Real-time timecode display |

### 12.3. Program Monitor

Section displaying the current Program and Preview sources.

- **M/E switcher** — select the Mix/Effect block (M/E 1, M/E 2, etc.) for multi-block switchers.
- Display of current **Program** and **Preview** input names.
- Real-time tally (red = Program, green = Preview).

### 12.4. Inputs Tab — Input Control

Paginated list of ATEM external inputs with tally indicators.

#### Available for each input:

| Action | Description |
|--------|-------------|
| **Program** | Send input to Program (red tally) |
| **Preview** | Send input to Preview (green tally) |
| **Cut** | Instant Cut transition to this input |
| **Auto** | Auto transition to this input |

- Color-coded tally border: **red** (in Program), **green** (in Preview).
- Input name and type display.
- Pagination for switchers with many inputs.

### 12.5. Scheduler Tab — Device Schedule

Compact list of scheduled tasks for the ATEM device (same layout as vMix scheduler tabs).

- Display of upcoming tasks: time, function, parameters, status.
- Time-until-next-task indicator.
- **Open Scheduler** button — navigate to the full scheduler page.

### 12.6. Card Footer

| Element | Description |
|---------|-------------|
| **🔒 Lock** | Default state: ON. Protects against accidental actions. Click to toggle |
| **🔔 Notifications** | Enable/disable notifications for this device (green — on, gray — off) |
| **⚠ Errors** | Display of current connection errors (in red) |
| **⏳ Spinner** | Loading indicator while an operation is in progress |
| **🔘 Connection Toggle** | Enable/disable connection to the switcher |

#### Built-in Command Feedback

When a command is executed (via UI, scheduler, or shortcut), the card footer displays a brief feedback message:
- **✓ CommandName** — success (auto-hides after 3 seconds).
- **✗ CommandName: error** — error with details.

#### Notifications

The ATEM card supports Windows Toast notifications for critical state changes:

| Category | Trigger |
|----------|---------|
| **Streaming** | Streaming started / stopped |
| **Recording (Disk)** | USB recording started / stopped |
| **Recording (HyperDeck)** | HyperDeck recording started / stopped |
| **DSK** | Downstream Keyer on-air state change |
| **Timecode** | Timecode-related events |

---

## 13. ATEM Command Catalog

ATEM devices provide a full command catalog for use with the **Task Scheduler** and **Shortcuts**. Commands are organized into 8 categories:

### Command Categories

| Category | Functions | Parameters |
|----------|-----------|------------|
| **Mix Effect** | Cut, AutoTransition, SetProgramInput, SetPreviewInput, SetTransitionPosition | MeIndex, InputId, Position |
| **Fade to Black** | FadeToBlack, SetFadeToBlackRate, SetFadeToBlackFullyBlack | MeIndex, Rate, FullyBlack |
| **Downstream Key** | SetOnAir, ToggleOnAir, PerformAutoTransition, SetTie | DskIndex, OnAir, Tie |
| **Camera Control** | StartRecording, StopRecording, StartRecordingForAllCameras, StopRecordingForAllCameras | Destination (camera address 0–254, broadcast 255) |
| **HyperDeck** | Record, Stop, Play, RecordAll, StopAll | HyperDeckId |
| **Streaming** | StartStreaming, StopStreaming | — |
| **Recording** | StartRecording, StopRecording, SwitchDisk | — |
| **Timecode** | ResetTimeCode | — |

### ATEM Feedback Events (Shortcuts)

When using ATEM devices with Shortcuts (external controller integration), the following feedback events are available:

| Category | Events |
|----------|--------|
| **Global** | Streaming, Recording, FadeToBlack, Transition, DSKOnAir |
| **Input-bound** | InputProgram, InputPreview |
| **HyperDeck** | HyperDeckRecord, HyperDeckPlay |

---

<a id="watch-rules"></a>
## 14. Watch Rules (Watchdog)

The **Watchdog** is a real-time rule engine that monitors your vMix devices and reacts **instantly** when something goes wrong on air. Instead of relying on a human to notice that recording stopped or a stream dropped, the Watchdog catches it for you — and can even fix it automatically.

> [!TIP]
> **Why this matters:** In a multi-machine broadcast, the operator watching the main mix may not notice that a replay server stopped recording, or that a graphics node lost its stream. A single missed recording can mean hours of lost footage with no way to recover. The Watchdog eliminates this risk.

**Currently supported devices:** vMix only.

---

### 14.1. Rule Structure

Every watch rule answers three questions:

| Component | Question | Example |
|-----------|----------|---------|
| **Trigger** | *WHEN to check?* | When the "Slate" input leaves Program |
| **Conditions** | *WHAT should be true?* | Recording is ON, Streaming is ON |
| **Action** | *WHAT to do if violated?* | Send alert / Auto-fix and alert |

Additional parameters:

| Parameter | Default | Description |
|-----------|---------|-------------|
| **Device** | All devices | Limit the trigger to a specific vMix instance, or leave blank for all |
| **Condition Logic** | All | **All** = every condition must be met; **Any** = at least one must be met |
| **Cooldown** | 30 sec | Minimum interval between repeated alerts for the same rule + device pair |
| **Enabled** | Yes | Disabled rules are stored but not evaluated |

---

### 14.2. Triggers

Triggers fire when a specific **input transition** happens in vMix:

| Trigger | Fires when… |
|---------|-------------|
| `OnTransitionIn` | An input **enters** Program (PGM) |
| `OnTransitionOut` | An input **leaves** Program (PGM) |
| `OnOverlayIn` | An input **appears** in an Overlay channel (1–4+) |
| `OnOverlayOut` | An input **disappears** from an Overlay channel (1–4+) |

**Input matching** — three modes:

| Mode | Match logic | Best for |
|------|-------------|----------|
| **By Name** | Case-insensitive substring of the input title | Naming conventions across machines (e.g. all slates named "Slate") |
| **By Number** | Exact input number | Fixed input layouts |
| **By Key** | Exact vMix input key (GUID) | Single-device rules with guaranteed uniqueness |

For Overlay triggers, you can optionally specify the **channel number** (1–4+). Leave blank to match any overlay channel.

---

### 14.3. Conditions

Conditions define the **expected state** of the device when the trigger fires:

| Condition | Checks |
|-----------|--------|
| `Recording` | Recording is active |
| `Streaming` | At least one stream channel is active |
| `External` | External Output is enabled |
| `Fullscreen` | Fullscreen output is enabled |
| `MultiCorder` | MultiCorder is active |
| `Master` | Master audio bus is NOT muted |

Each condition has an **Expected State** (`true` = should be ON, `false` = should be OFF). If the actual device state doesn't match the expected state, the condition is **violated**.

---

### 14.4. Actions

| Action | Behavior |
|--------|----------|
| **Send Alert** | Toast notification + external alert channels (Telegram, etc.) |
| **Auto-Fix and Alert** | Automatically sends the corrective vMix command (e.g. `StartRecording`), then sends a notification confirming the fix |
| **Execute Command** | Sends an arbitrary command from the vMix Command Catalog |

> [!IMPORTANT]
> **Auto-Fix** can save your broadcast. If the Watchdog detects that recording stopped on a replay node, it sends `StartRecording` before the operator even notices. The notification confirms the fix was applied — no footage lost.

**Violation lifecycle:**
1. Trigger fires → conditions evaluated → violation detected → action executed → `Violated` event.
2. Violation stays **active** until all conditions are restored.
3. When conditions recover → `Resolved` event → violation cleared.

---

### 14.5. Cross-Device Monitoring

This is the Watchdog's most powerful feature. Each condition can target a **different device** than the one that fired the trigger.

> **Scenario:** You have 3 vMix machines — Main Mix, Replay Server, and Graphics Node. You want to ensure that when the "Show Open" input goes to air on the Main Mix, **all three machines** are recording.

How it works:
- The **trigger** fires on Main Mix ("Show Open" enters PGM).
- **Condition 1:** Recording = ON → checked on **Main Mix** (trigger device).
- **Condition 2:** Recording = ON → checked on **Replay Server** (cross-device, via `TargetDeviceId`).
- **Condition 3:** Recording = ON → checked on **Graphics Node** (cross-device).
- **Logic:** All.
- **Action:** Auto-Fix and Alert.

If Replay Server's recording has stopped, the Watchdog **automatically sends `StartRecording`** to the Replay Server and notifies you. The Main Mix operator doesn't need to switch KVMs or check each machine manually.

> [!NOTE]
> Cross-device checks use the **last known state** of each device. If a target device is disconnected or has not yet sent its first state update, the condition is skipped (not treated as a violation).

---

### 14.6. Examples

#### Example 1: "Ensure recording when going live"

> *When the slate leaves PGM, recording and streaming must be ON — otherwise auto-fix.*

| Field | Value |
|-------|-------|
| **Name** | Rec+Stream check — Main Mix |
| **Device** | Main Mix |
| **Trigger** | `OnTransitionOut`, match by name: `Slate` |
| **Conditions** | Recording = ON, Streaming = ON |
| **Logic** | All |
| **Action** | Auto-Fix and Alert |
| **Cooldown** | 30 sec |

**Result:** The moment the operator cuts away from the slate, if recording or streaming is off, VRC starts them automatically and sends a toast + Telegram alert.

#### Example 2: "Cross-device recording guard"

> *When any input enters PGM on the Main Mix, verify all nodes are recording.*

| Field | Value |
|-------|-------|
| **Name** | All-node REC guard |
| **Device** | Main Mix |
| **Trigger** | `OnTransitionIn`, match by name: *(any — leave blank or use a common prefix)* |
| **Conditions** | Recording = ON on **Main Mix**, Recording = ON on **Replay**, Recording = ON on **GFX** |
| **Logic** | All |
| **Action** | Auto-Fix and Alert |

**Result:** A single trigger on the Main Mix validates recording across the entire production. Any node that dropped recording gets restarted instantly.

#### Example 3: "Muted master alert"

> *When a specific camera goes to air, the master audio bus must not be muted.*

| Field | Value |
|-------|-------|
| **Name** | Master unmute — Camera 1 |
| **Trigger** | `OnTransitionIn`, match by name: `Camera 1` |
| **Conditions** | Master = ON |
| **Action** | Send Alert |
| **Cooldown** | 60 sec |

**Result:** If Camera 1 goes to PGM with master muted, the operator gets an immediate warning.

---

---

<a id="external-alerts"></a>
## 15. External Alert Channels

VRC can send notifications not only as local Windows toasts but also to **external messaging services**. Every VRC notification (recording started, connection lost, Watchdog violation, audio muted, etc.) is automatically forwarded to all configured alert channels.

This is managed by the **Composite Notification Service**, which wraps the local toast and dispatches alerts to external providers in parallel.

> [!TIP]
> **Use case:** You're away from the control desk (lunch break, setup in another room). A Telegram message on your phone tells you that the replay server lost its recording. You catch it in seconds, not after the show.

---

### 15.1. Supported Providers

You can create **multiple instances** of the same provider type (e.g., two Telegram bots for different teams).

| Provider | Transport | Setup required |
|----------|-----------|----------------|
| **Telegram** | Bot API | Bot token + Chat ID |
| **Discord** | Webhook | Webhook URL |
| **Slack** | Incoming Webhook | Webhook URL |
| **Microsoft Teams** | Incoming Webhook | Webhook URL |
| **VK Teams** | Bot API | Bot token + Chat ID |
| **Yandex Messenger** | Bot API | Bot token + Chat ID |
| **ntfy** | Push (ntfy.sh / self-hosted) | Server URL + Topic |
| **Custom Webhook** | HTTP POST | Endpoint URL |

Each provider instance has:
- **Display Name** — a human-readable label for UI and logs (e.g., "TG — Sound Engineer").
- **Enabled** toggle — disabled providers are stored but not used.
- **Test** button — sends a test message to verify credentials before going live.

---

### 15.2. Device & Category Filters

By default, a provider receives **all** notifications from **all** devices. You can narrow this with filters:

| Filter level | What it does |
|-------------|---------------|
| **Device filter** | Select which devices send alerts to this provider |
| **Category filter** (per device) | Select which event categories are forwarded (Recording, Streaming, Connection, WatchRuleViolation, Audio, etc.) |

**Example:** "TG — Sound Engineer" receives only `AudioMasterMute` and `AudioBusMute` events from the Main Mix. No recording or connection spam.

**Available categories:**

| Category | Source |
|----------|--------|
| `Connection` | Device connect / disconnect |
| `Recording` | Recording start / stop |
| `Streaming` | Stream start / stop |
| `MultiCorder` | MultiCorder start / stop |
| `External` | External output on / off |
| `Fullscreen` | Fullscreen output on / off |
| `Replay` | Instant Replay events |
| `PlayList` | Playlist events |
| `Overlay` | Overlay in / out |
| `AudioMasterMute` | Master bus mute / unmute |
| `AudioBusMute` | Bus A–G mute / unmute |
| `AudioBusSendToMaster` | Bus send-to-master on / off |
| `AtemStreaming` | ATEM streaming start / stop |
| `RecordingDisk` | ATEM USB recording |
| `RecordingHyperDeck` | HyperDeck recording |
| `Dsk` | Downstream Key on / off |
| `Timecode` | Timecode reset |
| `WatchRuleViolation` | Watchdog rule violations |

---

### 15.3. Reliability: Retry & Circuit Breaker

External APIs can fail (network issues, rate limits, outages). VRC handles this automatically:

| Mechanism | Behavior |
|-----------|----------|
| **Retry** | Transient errors (HTTP 5xx, 429, timeouts) are retried up to **2 times** with exponential backoff (2 s → 4 s) |
| **No retry** | Client errors (HTTP 4xx except 429) fail immediately — usually a config problem |
| **Serialization** | Each provider processes one alert at a time (FIFO queue). Prevents flooding external APIs (e.g., Telegram rate limits) |
| **Circuit breaker** | After consecutive failures, the provider enters **Faulted** state — all alerts are skipped until the cooldown expires. This prevents log/network flooding when an API is down |
| **Auto-recovery** | After the cooldown, the circuit breaker enters **Half-Open** — one test delivery is allowed. If it succeeds, the provider is restored to **Healthy** |

---

### 15.4. Health Monitor

The **Alert Health Monitor** tracks delivery stats for every provider:

| Metric | Description |
|--------|-------------|
| **State** | `Healthy` → `Degraded` → `Faulted` |
| **Consecutive Failures** | Counter of failures in a row (resets on success) |
| **Total Sent / Failed / Skipped** | Lifetime counters since app start |
| **Last Success / Last Failure** | Timestamps (UTC) |
| **Last Error** | Error message from the most recent failure |
| **Circuit Open Until** | When the Faulted cooldown expires |

The UI shows a health indicator for each provider. If any provider is **Faulted**, the settings page highlights it. You can manually **Reset** a provider to clear the circuit breaker.

---

### 15.5. Alert Delivery Log

All external alert deliveries are logged to a dedicated file:

| File | Retention | Contents |
|------|-----------|----------|
| `Logs/Alerts/alerts-YYYYMMDD.log` | 30 days | Sent, failed (with attempt count), circuit breaker open/close events |

Example entries:
```
2026-01-15 14:32:01.123 [INF] Alert sent via 'TG — Director': "Main Mix" (Recording)
2026-01-15 14:32:03.456 [WRN] Alert FAILED via 'Discord — Crew': "Replay" — 429 Too Many Requests (attempt 1/3)
2026-01-15 14:32:05.789 [INF] Alert sent via 'Discord — Crew': "Replay" (Recording)
2026-01-15 15:00:12.000 [ERR] Provider 'Webhook — Monitor' FAULTED after 5 consecutive failures. Circuit breaker opened for 300s.
2026-01-15 15:05:12.100 [INF] Provider 'Webhook — Monitor' RESTORED — circuit breaker closed.
```

---

<a id="faq"></a>
## ❓ FAQ & Troubleshooting

### VRC cannot connect to vMix
- Verify that vMix is running and **Web Controller is enabled** (vMix Settings → Web Controller).
- Double-check the IP address and port (default HTTP: `8088`, TCP: `8099`).
- Ensure the Windows Firewall on the vMix machine allows inbound connections on that port.
- Use the **Probe** button in the Add/Edit device dialog to test connectivity before saving.

### Card buttons don’t respond to clicks
- Controls are **locked by default** to prevent accidental on-air actions.
- Click the **🔒 Lock icon** in the card footer to unlock the card.

### WMI monitoring shows no data
- Run the PowerShell setup scripts from VRC Settings → WMI (see [Section 4](#4-pc-health-monitoring)).
- Use the correct credential format: Workgroup → `username`; Domain → `DOMAIN\username` or `.\username`.
- Ensure TCP port `135` and the dynamic RPC range (`49152–65535`) are open on your network.

### Certificate fails to install
- Run the certificate installer as **Administrator** (right-click → Run as administrator).
- Ensure you place it in **Local Machine → Trusted People** (not Current User).

### Some indicators (Multicorder, Replay, GO) are missing
- These features depend on your **vMix edition and version**.
- Multicorder and Replay are only available in higher vMix editions.
- The **GO** button requires **vMix v29+**; earlier versions show **QuickPlay** instead.

### Notifications are not appearing
- Check **Settings → Notifications** and ensure the mode is not set to *Off*.
- Confirm Windows system notifications for VRC are allowed (Windows Settings → System → Notifications).

### VRC cannot connect to the ATEM switcher
- Ensure **Blackmagic ATEM Software Control** is installed on the VRC machine. VRC uses its COM SDK components to communicate with the switcher.
- Verify the IP address (default ATEM IP: `192.168.10.240`).
- Ensure UDP port `9910` is not blocked by a firewall between VRC and the switcher.
- Use the **Probe** button (ICMP ping) to check network reachability before saving.
- If you see "Incompatible firmware", update the ATEM firmware or ATEM Software Control to a compatible version.

### ATEM features (Streaming, Recording, HyperDeck) are not displayed
- Feature availability depends on **your ATEM switcher model**.
- Streaming and USB Recording indicators are only shown for models with a built-in encoder (ATEM Mini series, etc.).
- HyperDeck indicators appear only when HyperDecks are connected to the switcher.
- Camera Recording requires Blackmagic cameras connected via SDI.

### ATEM error "COM class not registered"
- This means **ATEM Software Control** is not installed or its COM components were not registered correctly.
- Reinstall Blackmagic ATEM Software Control and restart VRC.
