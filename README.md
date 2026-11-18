# ASH MobileData

ASH MobileData is a lightweight, customizable Android utility designed to automate and control **Airplane Mode** and **Mobile Data** toggling based on your specific network conditions and rules. Whether you need to refresh your mobile IP, recover stalled connections, or enforce data limits, you can build tailored configurations to handle it automatically.

> ⚠️ **Important Notice:** This is a closed-source project. This repository contains no source code and is used exclusively for distributing official release binaries (APKs). **Feature suggestions and feedback are welcome**, however pull requests and external code contributions will not be accepted.

---

## 🛠️ Core Features

Create multiple custom configurations, choose whether each profile controls **Airplane Mode** or **Mobile Data**, and select one of five automated trigger modes:

* **Timer**
  * Toggles the selected mode on and off automatically after a user-defined constant delay (in milliseconds).

* **Ping 1 (Traffic Monitor)**
  * Monitors mobile data upstream and downstream traffic.
  * Triggers toggling if both—or either, based on your configuration—drop to zero across a specified number of checks.

* **Ping 2 (Connectivity Check)**
  * Verifies active internet availability by checking target websites.
  * Triggers toggling after a specified number of consecutive failed connection attempts.

* **Consumption**
  * Tracks mobile data usage and triggers toggling once consumption reaches a user-defined threshold.

* **Slow Speed**
  * Monitors real-time network speed.
  * Triggers toggling when data speed stays below a specified threshold across a user-defined number of consecutive checks.

---

## 🔐 Permissions & Requirements

Depending on which mode you choose to automate, ASH MobileData requires specific system permissions to toggle network states on modern Android versions:

* **For Airplane Mode (Choose one method):**
  * **Assistant Method:** Set ASH MobileData as your device's **Default Digital Assistant App** and enable **Display over other apps** (`SYSTEM_ALERT_WINDOW`) *(optional, recommended for smoother execution)*.
  * **Shizuku Method:** Grant permission via **Shizuku** (no root required).
  * *(Note: Native Root access support is currently under consideration for a future update.)*

* **For Mobile Data:**
  * **Shizuku Method:** Grant permission via **Shizuku** (required to toggle mobile data programmatically).
  * *(Note: Native Root access support is currently under consideration for a future update.)*

---

## 💾 Installation

The source code for this application is private. To use ASH MobileData, download the compiled package directly from this repository:

1. Navigate to the **Releases** section on the right side of this page.
2. Download the latest `.apk` file.
3. Transfer the file to your Android device and install it (ensure **Install from Unknown Sources** is enabled in your device settings).
4. Open the app and grant the required permissions (Default Assistant / Overlay or Shizuku) for your chosen mode.

---

## 💡 Suggestions & Feedback

While the codebase is private and pull requests are closed, user ideas are always welcome. If you have a feature suggestion or improvement idea, feel free to open an entry in the **Issues** tab.

## 📄 License

All rights reserved. This application is provided as-is without an open-source license. Unauthorized distribution, modification, or reverse engineering of the release binaries is prohibited.
