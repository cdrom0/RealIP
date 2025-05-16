# RealIP

A browser-based tool that leverages WebRTC to detect local and public IP addresses using ICE candidates via a STUN server.

---

## ✅ Features

* 📡 **STUN Server Integration:** Uses `stun.l.google.com:19302` to discover public IP addresses.
* 🔍 **Local IP Detection:** Identifies local network IPs using WebRTC ICE candidates.
* 🛠️ **Dynamic Table Rendering:** Displays detected IPs, ports, protocols, and candidate types in a clean, tabular format.
* 📦 **No External Libraries:** Pure HTML, CSS, and JavaScript implementation.

---

## 🛠️ Installation

1. **Clone the repository:**

   ```bash
   git clone https://github.com/cdrom0/RealIP.git
   cd RealIP
   ```

2. **Open the HTML file:**

   * Open `realip.html` directly in your browser.
   * Alternatively, run a local server for enhanced compatibility:

     ```bash
     python -m http.server
     ```
   * Then, access the tool at: `http://localhost:8000`

---

## 🧪 Usage

* 🌐 **Open the HTML file in a browser.**
* 🚀 **Wait for WebRTC to gather ICE candidates.**
* 📋 **View the detected IPs and associated metadata in the table.**

### 💻 Example Output:

| IP Address   | Port  | Protocol | Candidate Type |
| ------------ | ----- | -------- | -------------- |
| 192.168.1.10 | 53725 | udp      | host           |
| 203.0.113.5  | 19302 | udp      | srflx          |

---

## 📝 How It Works

* ✅ **STUN Server:** The tool sends WebRTC requests to a STUN server to discover public-facing IPs.
* 📦 **ICE Candidates:** Captures ICE candidates and extracts IP, port, protocol, and candidate type.
* 🛠️ **DOM Manipulation:** Populates the detected information in the HTML table dynamically.

---

## ⚠️ Privacy Note

* This tool **does not send data to any third-party server.**
* All IP detection is performed locally within the browser.
