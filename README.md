# 🎵 cBPM v.2 - Crowd-based BPM Detector

**cBPM** (Crowd-based BPM) is an open-source experiment that captures the *collective rhythm* of a crowd by letting users tap to the beat during live music events. Taps are aggregated in real time, producing an accurate, community-driven BPM display.

Built with ultra-fast and lightweight technologies — no bloated frameworks, just **HTMX**, **Animora**, and **Rust**.

[![cBPM Demo](https://img.youtube.com/vi/hRP4IMtft4E/0.jpg)](https://www.youtube.com/watch?v=hRP4IMtft4E)

---

## ✨ Features

- 🖱️ Tap-based beat input from audience
- ⏱️ Real-time BPM aggregation and display
- 📲 Mobile-first responsive interface
- ⚡ Built using [HTMX](https://htmx.org) and [Animora](https://github.com/makalin/animora)
- 🔌 Rust backend with WebSockets and Axum

---

## 🛠️ Stack Overview

| Layer      | Technology            |
|------------|------------------------|
| Frontend   | HTMX + Animora (CSS)   |
| Backend    | Rust + Axum + WebSocket|
| Database   | SQLite (or Postgres)   |
| Hosting    | Static + binary server |

---

## 📁 Project Structure

```

cbpm/
├── frontend/
│   ├── index.html         # Main UI
│   ├── app.js             # Tap logic
│   ├── animora.css        # Custom utility-first CSS
│   └── assets/
├── backend/
│   ├── src/
│   │   └── main.rs        # Rust server with Axum
│   └── Cargo.toml
└── README.md

````

---

## 🚀 Getting Started

### 🖥 Frontend (Static)

You can run this with any HTTP server.

```bash
cd frontend
python3 -m http.server 8080
# Visit http://localhost:8080
````

### 🦀 Backend (Rust)

Make sure you have [Rust](https://www.rust-lang.org/tools/install) installed.

```bash
cd backend
cargo build --release
./target/release/cbpm_backend
```

---

## ⚙️ How It Works

1. Users open the web app and tap in rhythm.
2. Each tap is sent to the backend via HTMX requests or WebSockets.
3. Server calculates rolling BPM average from all active users.
4. Visual BPM display is updated in real time.

---

## 📸 Screenshots

> Add visuals or demo GIFs in `/frontend/assets/` and reference them here.

---

## 📜 License

MIT © [Mehmet Akalın](https://github.com/makalin)

---

## 🔗 External Links

* 🔊 [Frange – Aura Album Release](https://muzikonair.com/aura-adli-solo-albumunu-cikaran-frange-joker-no-19da/)
* 🎫 [Event Page on RA](https://ra.co/events/768088)
* 💻 [Legacy CBPM App](https://cbpm.soft112.com/)
* 💡 [Animora CSS Framework](https://github.com/makalin/animora)

---

## 🤝 Contribute

Contributions are welcome! Fork the repo, improve it, and open a PR.
