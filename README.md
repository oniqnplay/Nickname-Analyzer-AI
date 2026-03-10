# 🧠 Nickname Analyzer v1.0

> **AI-powered name personality decoder — runs 100% in your browser, no API needed.**

Masukkan nama kamu dan temukan energi, vibe, arketipe, dan kepribadian tersembunyi di baliknya — secara instan, menggunakan AI heuristik berbasis analisis fonetik dan linguistik.

![Status](https://img.shields.io/badge/status-stable-brightgreen?style=flat-square)
![License](https://img.shields.io/badge/license-MIT-blue?style=flat-square)
![Stack](https://img.shields.io/badge/built%20with-HTML%20%2B%20Vanilla%20JS-orange?style=flat-square)
![AI](https://img.shields.io/badge/AI-heuristic%20engine-8b5cf6?style=flat-square)
![No API](https://img.shields.io/badge/API-none%20required-00c853?style=flat-square)

---

## ✨ Features

| Fitur | Deskripsi |
|---|---|
| 🤖 **AI Heuristic Engine** | Analisis fonetik otomatis — vokal, konsonan, power letters, dan pola suku kata |
| ⚡ **Energi Nama** | Score 0–100% berdasarkan struktur dan resonansi fonetik |
| ✨ **Vibe Profile** | 8 profil: Elegan, Klasik, Energik, Misterius, Kreatif, Minimalis, Tangguh, Hangat |
| 🎭 **Arketipe** | 8 tipe: The Visioner, Guardian, Creator, Explorer, Sage, Hero, Jester, Ruler |
| 🏷️ **Sifat Dominan** | 3–4 badge trait unik per nama |
| 🔢 **Numerologi** | Kalkulasi nilai numerologi 1–9 dengan maknanya |
| 📛 **Nickname Suggestions** | Rekomendasi nickname ideal + panggilan formal |
| 🌙 **Dark / Light Mode** | Toggle tema dengan preferensi tersimpan |
| 🔒 **100% Private** | Tidak ada data yang keluar dari browser kamu |

---

## 🧠 Cara Kerja AI-nya

Engine ini menggunakan **Heuristic Analysis** murni JavaScript — tanpa API, tanpa backend:

```
INPUT nama → Hitung rasio vokal/konsonan
           → Deteksi power letters (S, X, Z, K, R)
           → Analisis panjang & pola ending
           → Kalkulasi numerologi (digit reduction)
           → Seeded RNG → output konsisten per nama
OUTPUT → Energy%, Vibe, Archetype, Traits, Insight
```

**Contoh logika:**
- Nama pendek (≤4 huruf) → Tegas & powerful (+15 poin)
- Banyak huruf `A`, `O` → Terbuka & ramah (+vokal bonus)
- Mengandung `S`, `X`, `Z` → Modern & tajam (+power bonus)
- Berakhiran konsonan → Formal & profesional (+resonansi)

Hasilnya **deterministik** — nama yang sama selalu menghasilkan output yang sama.

---

## 🚀 Cara Pakai

### Buka Langsung di Browser
```
Ctrl + O → pilih index.html
```
Atau drag & drop file `index.html` ke Chrome/Firefox.

### Serve Lokal
```bash
python -m http.server 8080
# Buka: http://localhost:8080
```

### Deploy ke GitHub Pages (Gratis)
1. Push repo ini ke GitHub
2. **Settings → Pages → Source: `main` branch → `/` (root)**
3. Live di: `https://username.github.io/nickname-analyzer`

### Deploy ke Google Apps Script
1. Buka [script.google.com](https://script.google.com)
2. Buat project baru → `File → New → HTML File`
3. Paste isi `index.html`
4. **Deploy → New Deployment → Web App**
5. Akses lewat link Web App yang diberikan

---

## 🛠️ Tech Stack

| Layer | Teknologi |
|---|---|
| Structure | HTML5 |
| Logic | Vanilla JavaScript (ES6+) |
| Styling | Tailwind CSS (CDN) + Custom CSS |
| Icons | Material Symbols (Google) |
| Fonts | Inter (Google Fonts) |
| AI Engine | Client-side Heuristic (no API) |
| Storage | `localStorage` (dark mode only) |

---

## 📁 Struktur File

```
nickname-analyzer/
└── index.html       # Seluruh app dalam satu file
└── README.md        # Dokumentasi ini
```

---

## 💡 Use Cases

- **Personal Branding** — Analisis nama profil LinkedIn atau username media sosial
- **Orang Tua** — Cek kesan nama sebelum diberikan ke anak
- **Content Creator** — Pilih nama yang punya vibe paling kuat untuk channel/akun
- **Developer** — Inspirasi AI logika ringan tanpa API

---

## 📄 License

MIT License — bebas digunakan, dimodifikasi, dan didistribusikan.

---

<p align="center">
  Made with ⚡ by <strong>Nickname Analyzer</strong> · No server. No API. No data collected.
</p>
