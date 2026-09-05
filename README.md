# ✦ Aether Frame

**Aether Frame** is a gesture-controlled spatial interface that lets you create, move, and resize virtual panels using your hands and webcam.

Built with **JavaScript, Vite, Electron, and MediaPipe Hands**.

---

## ✨ Features

* 🖐️ Real-time hand tracking
* ✌️ Supports up to two hands
* 🔲 Create rectangles/panels using hand gestures
* ↔️ Resize panels using both hands
* 🖱️ Move panels using one-hand pinch
* 📐 Resize panels from corners
* 🖥️ Mouse mode available as an alternative
* ⚡ Smooth high-refresh-rate rendering
* 📷 Webcam-based tracking
* 🔒 Hand tracking runs locally on your computer
* 🌐 Works offline after installation

---

# 🚀 How to Run Aether Frame

## Requirements

Before running the project, install:

* **Windows 10 / Windows 11**
* **Node.js 20 or newer**
* **VS Code**
* A working **webcam**

You can check Node.js by opening Command Prompt or the VS Code terminal and running:

```bash
node -v
```

And:

```bash
npm -v
```

---

# 💻 Run in VS Code

### 1. Download or clone the repository

If you downloaded the project as a ZIP:

1. Extract the ZIP file.
2. Open the extracted **Aether Frame** folder.
3. Right-click inside the folder.
4. Select **Open with Code**.

Or open VS Code and select:

```text
File → Open Folder
```

Then select the Aether Frame project folder.

---

### 2. Open the VS Code terminal

Inside VS Code:

```text
Terminal → New Terminal
```

Make sure the terminal is inside the folder containing:

```text
package.json
```

---

### 3. Install dependencies

Run:

```bash
npm install
```

This installs all required packages including:

* Electron
* Vite
* MediaPipe Hands
* Electron Builder
* Concurrently
* Wait-on

Wait until installation finishes successfully.

---

### 4. Start Aether Frame

Run:

```bash
npm run desktop
```

Aether Frame should automatically launch as a desktop application.

---

# 📷 Enable Hand Tracking

When Aether Frame opens:

1. Click **Initialize Vision**
2. Allow camera/webcam access
3. Place your hands inside the camera frame
4. Keep your hands clearly visible

For better tracking:

* Use good lighting
* Keep your hands inside the webcam frame
* Avoid very dark backgrounds
* Face your palms toward the camera

---

# 🖐️ Gesture Controls

| Gesture                                  | Action                 |
| ---------------------------------------- | ---------------------- |
| Pinch thumb + index finger on both hands | Start creating a panel |
| Move both pinched hands apart/together   | Resize the new panel   |
| Release either hand                      | Place the panel        |
| Pinch inside an existing panel           | Move the panel         |
| Pinch near a panel corner                | Resize the panel       |

---

# ⚡ Fastest Way to Start

The project includes:

```text
START-AETHER-FRAME.bat
```

On Windows you can simply double-click:

```text
START-AETHER-FRAME.bat
```

If dependencies are not installed yet, the launcher will automatically run:

```bash
npm install
```

and then launch:

```bash
npm run desktop
```

---

# 🌐 Run Only the Web Version

If you don't want to launch Electron, you can run the Vite version:

```bash
npm run dev
```

Then open:

```text
http://127.0.0.1:5173
```

in your browser.

Allow camera permissions when requested.

---

# 🪟 Build Aether Frame as a Windows App

Aether Frame can also be converted into an installable Windows application.

Run:

```bash
npm install
```

Then:

```bash
npm run dist:win
```

Or simply double-click:

```text
BUILD-WINDOWS-APP.bat
```

After the build finishes, open:

```text
release/
```

You should find the generated Windows installer and portable `.exe` there.

---

# 📂 Project Structure

```text
Aether-Frame/
│
├── electron/
│   ├── main.cjs
│   └── preload.cjs
│
├── public/
│   └── mediapipe/
│
├── scripts/
│   └── sync-mediapipe.mjs
│
├── src/
│   ├── main.js
│   └── style.css
│
├── index.html
├── package.json
├── package-lock.json
├── vite.config.js
│
├── START-AETHER-FRAME.bat
├── BUILD-WINDOWS-APP.bat
│
└── README.md
```

---

# 🛠️ Available Commands

### Install dependencies

```bash
npm install
```

### Start web development server

```bash
npm run dev
```

### Start desktop application

```bash
npm run desktop
```

### Build frontend

```bash
npm run build
```

### Preview production build

```bash
npm run preview
```

### Build Windows installer + portable EXE

```bash
npm run dist:win
```

---

# ❗ Common Problems

## `npm is not recognized`

Install Node.js and restart VS Code.

Then check:

```bash
node -v
npm -v
```

---

## Camera is not working

Make sure Windows camera permissions are enabled.

Go to:

```text
Settings
→ Privacy & security
→ Camera
```

Enable camera access for desktop apps.

Then restart Aether Frame.

---

## `node_modules` error

Delete:

```text
node_modules
```

and run:

```bash
npm install
```

again.

---

## App doesn't open

Try:

```bash
npm run desktop
```

from the VS Code terminal so you can see the exact error.

---

## Port 5173 already in use

Close any previous Vite/Aether Frame terminal and run:

```bash
npm run desktop
```

again.

---

# 🎯 Recommended Start Command

For normal development:

```bash
npm install
npm run desktop
```

After the first installation, you normally only need:

```bash
npm run desktop
```

or simply double-click:

```text
START-AETHER-FRAME.bat
```

---

# 🔒 Privacy

Aether Frame performs hand tracking locally using MediaPipe.

Camera frames are used for gesture detection and are not intended to be uploaded to an external server.

---

# 👨‍💻 Author

**Kritagya Verma**

---

# 📄 License

This project is licensed under the **MIT License**.

---

## ✦ Aether Frame

**Move your hands. Shape your space.**
