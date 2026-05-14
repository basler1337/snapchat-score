# 📸 Snapchat Score Spammer

Automatically send snaps to your entire friends list to farm your Snapscore — fast and easy to set up.

> ⚠️ **Warning:** This tool violates Snapchat's Terms of Service. Your account may get banned. Use a **secondary/test account** to spam your main account. You have been warned.

---

## ✅ Requirements

Before you start, make sure you have the following installed:

- [Python 3.11 or newer](https://www.python.org/downloads/)
- [Google Chrome](https://www.google.com/chrome/) (must be installed!)

---

## 📥 Installation

### Step 1 — Download the project

Download or clone this repository and extract it to a folder on your Desktop (or anywhere you like).

### Step 2 — Install Python

1. Go to https://www.python.org/downloads/ and download Python 3.11 or newer.
2. Run the installer.
3. **IMPORTANT:** On the first screen of the installer, check the box that says ✅ **"Add python.exe to PATH"** — without this, nothing will work!
4. Click **Install Now** and wait for it to finish.

### Step 3 — Install Google Chrome

If you don't have Google Chrome installed, download and install it from:
https://www.google.com/chrome/

---

## ⚙️ Setup

### Step 4 — Edit your login credentials

Open `main.py` in any text editor (e.g. Notepad, VS Code).

Scroll to the very **bottom** of the file and find this line:

```python
snapchat = Snapchat(username="YOUR_USER", password="YOUR_PASSWORD")
```

Replace `YOUR_USER` with your Snapchat username and `YOUR_PASSWORD` with your password.

**Example:**
```python
snapchat = Snapchat(username="myaccount123", password="mysecretpass")
```

Save the file.

---

## 🚀 Running the Tool

### Step 5 — Open a terminal in the project folder

1. Open the folder where you extracted the project files.
2. Hold **Shift** and **right-click** inside the folder.
3. Select **"Open PowerShell window here"** or **"Open in Terminal"**.

### Step 6 — Install dependencies (only needed once)

Copy and paste this command into the terminal and press **Enter**:

```bash
py -m pip install selenium webdriver-manager undetected-chromedriver
```

Wait until everything is installed successfully.

### Step 7 — Start the script

Run the following command:

```bash
py main.py
```

A **Google Chrome window** will open automatically and navigate to Snapchat Web.

### Step 8 — Log in manually

In the Chrome window that opened, **log into your Snapchat account manually**. The script will wait for you to finish logging in before it starts.

Once you are logged in, the script will start sending snaps to your friends list automatically. 🎉

---

## 🔄 How It Works

- The script opens Snapchat Web in Chrome and logs in using cached session data.
- It loops through your entire friends list and sends a snap to each person.
- Between batches, it waits a random amount of time (30 seconds to 5 minutes) to avoid detection.
- Every 4 hours, it takes a longer break (10–15 minutes) to simulate natural usage.
- If an error occurs (e.g. session expired), it will automatically try to re-login.

---

## ❓ Troubleshooting

| Problem | Solution |
|---|---|
| `'pip' is not recognized` | Use `py -m pip install ...` instead of `pip install ...` |
| `'python' is not recognized` | Use `py main.py` instead of `python main.py` |
| `Cannot find Chrome binary` | Install Google Chrome from https://www.google.com/chrome/ |
| Script opens but does nothing | Make sure you log into Snapchat in the Chrome window that opens |
| Account got banned | Use a secondary/throwaway account — this tool violates Snapchat's ToS |

---

## ⭐ Support

If this tool helped you, consider leaving a **star** on the repository — it helps with future updates and improvements!
