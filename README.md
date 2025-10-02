# SignBot 🪧🤖

**SignBot** is a Minecraft automation tool designed to scan signs in loaded chunks, filter out unwanted ones, and send Baritone commands to visit valid sign locations. It’s built for Fabric mod environments and optimized for modular control and persistent logging.

---

## 🔍 Features

- ✅ Scans all loaded sign blocks in the world
- ✅ Filters out:
  - Blank signs
  - Signs starting with `codysmile11` followed by `was here:)`
- ✅ Queues valid signs for Baritone pathfinding
- ✅ Sends `#goto` commands one at a time
- ✅ Logs all actions to `signbot-log.txt`
- ✅ Displays a fun chat summary after each scan

---

## 🧠 Control Flow

- **Toggle scanning** with a keybind or method call (`toggleScanning()`)
- **Scan once**, then auto-pause to prevent memory overload
- **Queue valid signs** for dispatch
- **Dispatch signs manually** using `dispatchNextSign()` or via timer
- **Chat summary** includes total signs, Cody tags ignored, blanks skipped, and valid signs queued

---

## 📦 Installation

1. Clone this repo:
   ```bash
   git clone https://github.com/yourusername/SignBot.git
