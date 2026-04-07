# CQTS+ Update Guide

Follow these steps to update CQTS+ to a new version.

---

## 1. Stop Services from the Dashboard

Open the CQTS+ web interface and stop both services:

1. Navigate to the **Process Control** panel
2. Click **Stop** on the **Executor**
3. Click **Stop** on the **Orchestrator**
4. Wait for both to show a stopped/idle status

---

## 2. Close the Web Interface

Close the CQTS+ dashboard browser tab or window.

---

## 3. Kill the Background Process

Terminate the `cqts-start` background process:

**Option A — Task Manager**
1. Press `Ctrl + Shift + Esc`
2. Find `cqts-start.exe` under the **Processes** tab
3. Right-click → **End task**

**Option B — Command Prompt**
```cmd
taskkill /IM cqts-start.exe /F
```

---

## 4. Install the New Version

1. Download all `.zip` files from the [latest release](https://github.com/wonderjimmy/cqts-plus-release/releases/latest)
2. Extract each `.zip` into your CQTS+ installation folder, replacing the existing files

Your configuration files and strategy data are stored separately and will not be affected.

---

## 5. Launch CQTS+

Run `cqts-start.exe` from your installation folder.

The dashboard will open automatically in your browser.

---

## 6. Resume Trading

Once your strategy settings have been reviewed and confirmed:

1. Navigate to the **Process Control** panel
2. Start the **Orchestrator**
3. Start the **Executor**

CQTS+ is now running on the new version.
