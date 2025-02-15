<h1 align="center">ðŸ¤– BlackboxAI to Telegram Bot</h1>
<p align="center">
  <b>Integrasi API BlackboxAI ke Bot Telegram</b><br>
  <i>Contributor: <a href="https://github.com/siputzx">siputzx</a> and BlackboxAI Team</i>
</p>

<p align="center">
  <img src="https://visitor-badge.glitch.me/badge?page_id=siputzx.blackboxai-telegram" alt="Visitors">
  <img src="https://img.shields.io/github/stars/siputzx/blackboxai-telegram?style=for-the-badge">
  <img src="https://img.shields.io/github/forks/siputzx/blackboxai-telegram?style=for-the-badge">
</p>

---

## âœ¨ Fitur
- ðŸ”¥ **Integrasi langsung dengan API BlackboxAI**  
- âš¡ **Respon cepat dan ringan menggunakan Telegraf**  
- ðŸ”„ **Dapat berjalan di berbagai platform**  
- ðŸ” **Keamanan terjamin dengan penggunaan API Key**  
- ðŸ›  **Mudah diinstal dan dikonfigurasi**  

---

## ðŸš€ Instalasi

### 1ï¸âƒ£ **Persyaratan Awal**
Sebelum menjalankan bot, pastikan kamu sudah menginstal **Node.js** versi terbaru:  
ðŸ”— [Download Node.js](https://nodejs.org/)

### 2ï¸âƒ£ **Clone Repository**
```bash
git clone https://github.com/siputzx/blbx-bot.git
cd blbx-bot
```

### 3ï¸âƒ£ **Install Dependency**
```bash
npm install
```

### 4ï¸âƒ£ **Konfigurasi Bot**
Buat file `.env` dan isi dengan:
```
TELEGRAM_BOT_TOKEN=your_telegram_bot_token
BLACKBOXAI_API_KEY=your_blackboxai_api_key
```

### 5ï¸âƒ£ **Menjalankan Bot**
```bash
node index.js
```

---

## ðŸ›  Cara Deploy di Berbagai Platform

### ðŸ”¹ **Termux (Android)**
```bash
pkg update && pkg upgrade
pkg install nodejs git
git clone https://github.com/siputzx/blbx-bot.git
cd blbx-bot
npm install
node index.js
```

### ðŸ”¹ **Replit**
1. Fork repo ini ke akun GitHub kamu  
2. Buat project baru di Replit dan pilih `Import from GitHub`  
3. Masuk ke **Secrets** â†’ Tambahkan `TELEGRAM_BOT_TOKEN` dan `BLACKBOXAI_API_KEY`  
4. Jalankan dengan `node index.js`

### ðŸ”¹ **Heroku**
```bash
heroku create
git push heroku main
heroku config:set TELEGRAM_BOT_TOKEN=your_token
heroku config:set BLACKBOXAI_API_KEY=your_key
heroku ps:scale web=1
heroku open
```

### ðŸ”¹ **Pterodactyl Panel**
1. Tambahkan **Egg Node.js** pada server  
2. Upload project ini ke **File Manager**  
3. Tambahkan environment variable di panel  
4. Jalankan server  

### ðŸ”¹ **VPS / Koyeb / RDP**
```bash
git clone https://github.com/siputzx/blbx-bot.git
cd blbx-bot
npm install
node index.js
```

---

## ðŸŒŸ Dukungan dan Kontribusi  
Jika kamu ingin berkontribusi, silakan **fork repository ini** dan buat **pull request**.  
Jangan lupa beri â­ di repo ini jika bermanfaat!

ðŸ“Œ **Tim BlackboxAI** dan **Contributor siputzx** siap membantu jika ada kendala.  

---

<p align="center">
  <b>ðŸš€ Made with â¤ï¸ by siputzx and BlackboxAI Team</b>
</p>
