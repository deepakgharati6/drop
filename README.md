# ByteShalaDrop 🚀

Ultra-fast, secure **peer-to-peer file sharing** web app built with **WebRTC + PeerJS**.
No Firebase. No database. No file storage on any server.

Files go **directly from device to device**.

---

## ✨ Features

* 🔗 **True P2P (WebRTC DataChannel)**
* 🔐 No Firebase, no backend, no tracking
* ⚡ Ultra-fast chunked file transfer (256KB chunks)
* 📶 Works on same network **and over internet**
* 🔢 Simple **4-digit PIN pairing**
* 📱 Mobile-friendly, responsive UI (TailwindCSS)
* 🧠 Smart buffer control (prevents browser crash)
* 🌙 Modern glassmorphism dark UI

---

## 🧠 How It Works

1. Each device generates a **random 4-digit PIN**
2. A PeerJS peer is created using:

   ```
   bs-drop-<PIN>
   ```
3. Sender enters receiver PIN
4. PeerJS handles signaling
5. WebRTC establishes direct connection
6. Files are sent in **binary chunks**

> Files are never uploaded to any server.

---

## 🛠 Tech Stack

* **HTML5**
* **TailwindCSS** (UI)
* **jQuery** (DOM handling)
* **PeerJS** (WebRTC signaling + abstraction)
* **WebRTC DataChannel** (actual file transfer)

---

## 🚀 Usage

### 1️⃣ Open the app on two devices

Host it locally or open via any static hosting:

```bash
php -S localhost:3000
```

or

```bash
npx serve .
```

---

### 2️⃣ Receiver

* Open the site
* Share the shown **4-digit PIN**

### 3️⃣ Sender

* Enter receiver PIN
* Click **Connect & Send**
* Select file

---

## 📦 File Transfer Details

* Chunk size: **256 KB**
* Buffer threshold: **2 MB**
* Progress tracked in real-time
* Automatic file reconstruction on receiver

---

## 🔒 Security Notes

* End-to-end encrypted by WebRTC
* No server file storage
* No logging
* No authentication required

---

## ⚠ Limitations

* Requires internet for PeerJS signaling
* Browser must support WebRTC
* Very large files (>5–10GB) depend on browser memory

---

## 📌 Future Improvements

* 🔍 Auto-discover devices on same LAN
* 📂 Multiple file / folder support
* 📊 Speed & ETA indicator
* 📱 Android WebView build
* 🔐 Optional PIN confirmation dialog

---

## 👨‍💻 Author

**Deepak Gharati**
ByteShala Private Limited

---

## 📄 License

MIT License — free to use, modify, and distribute.

---

### ⭐ If you like this project

Give it a star ⭐ on GitHub and share it 🚀
