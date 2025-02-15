# Blackbox.ai Telegram Bot

![Blackbox.ai Telegram Bot](https://socialify.git.ci/siputzx/blbx-bot/image?description=1&descriptionEditable=Integrate%20Blackbox.ai%20API%20with%20Telegram%20Bot&font=Inter&forks=1&issues=1&language=1&name=1&owner=1&pattern=Circuit%20Board&pulls=1&stargazers=1&theme=Dark)

<p align="center">
  <a href="https://github.com/siputzx/blbx-bot/stargazers"><img src="https://img.shields.io/github/stars/siputzx/blbx-bot?color=yellow&style=flat-square"></a>
  <a href="https://github.com/siputzx/blbx-bot/network/members"><img src="https://img.shields.io/github/forks/siputzx/blbx-bot?style=flat-square"></a>
  <a href="https://github.com/siputzx/blbx-bot/watchers"><img src="https://img.shields.io/github/watchers/siputzx/blbx-bot?style=flat-square"></a>
  <a href="https://github.com/siputzx/blbx-bot/issues"><img src="https://img.shields.io/github/issues/siputzx/blbx-bot?style=flat-square"></a>
  <a href="https://github.com/siputzx/blbx-bot/graphs/contributors"><img src="https://img.shields.io/github/contributors/siputzx/blbx-bot?style=flat-square"></a>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Node.js-43853D?style=for-the-badge&logo=node.js&logoColor=white" alt="Node.js">
  <img src="https://img.shields.io/badge/Telegram-2CA5E0?style=for-the-badge&logo=telegram&logoColor=white" alt="Telegram">
  <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black" alt="JavaScript">
</p>

## 📊 Repository Stats

![Repo Visitors](https://visitor-badge.laobi.icu/badge?page_id=siputzx.blbx-bot)
![Last Commit](https://img.shields.io/github/last-commit/siputzx/blbx-bot)
![Repo Size](https://img.shields.io/github/repo-size/siputzx/blbx-bot)

## 🌟 Features

- Seamless integration of Blackbox.ai API with Telegram
- Quick responses to user queries
- Support for code generation and assistance
- Easy deployment on multiple platforms
- Minimal resource requirements
- Modern and elegant interface

## 📋 Prerequisites

Before setting up the bot, ensure you have:

- [Node.js](https://nodejs.org/) (v14 or newer)
- Blackbox.ai API key
- Telegram Bot Token (from [@BotFather](https://t.me/BotFather))

## 🚀 Installation and Setup

### 1. Clone the repository

```bash
git clone https://github.com/siputzx/blbx-bot.git
cd blbx-bot
```

### 2. Install dependencies

```bash
npm install
```

### 3. Configure environment variables

Create a `.env` file in the root directory with the following content:

```
BOT_TOKEN=your_telegram_bot_token
BLACKBOX_API_KEY=your_blackbox_api_key
```

### 4. Start the bot

```bash
npm start
```

## 🖥️ Deployment Guidelines

### Termux (Android)

1. Install Termux from F-Droid
2. Run the following commands:

```bash
pkg update && pkg upgrade
pkg install nodejs git
git clone https://github.com/siputzx/blbx-bot.git
cd blbx-bot
npm install
# Create .env file with required values
npm start
```

### Replit

1. Create a new Replit project
2. Import from GitHub: `https://github.com/siputzx/blbx-bot.git`
3. Add secrets in Replit for `BOT_TOKEN` and `BLACKBOX_API_KEY`
4. Click Run button

### Heroku

1. Create a Heroku account and install Heroku CLI
2. Clone the repository locally
3. Initialize Heroku app:

```bash
heroku login
heroku create your-app-name
git push heroku main
heroku config:set BOT_TOKEN=your_telegram_bot_token
heroku config:set BLACKBOX_API_KEY=your_blackbox_api_key
```

### Pterodactyl Panel

1. Create a new Node.js server in your panel
2. Set startup command to `npm start`
3. Upload the repository files
4. Add environment variables in the Startup tab
5. Start the server

### VPS (Ubuntu/Debian)

1. Connect to your VPS via SSH
2. Install Node.js and npm:

```bash
sudo apt update
sudo apt install nodejs npm
git clone https://github.com/siputzx/blbx-bot.git
cd blbx-bot
npm install
# Create .env file with required values
npm start
```

### Koyeb

1. Sign up for a Koyeb account
2. Connect your GitHub account
3. Create a new app from the GitHub repository
4. Add environment variables:
   - `BOT_TOKEN`
   - `BLACKBOX_API_KEY`
5. Deploy the application

### cPanel (Not Recommended)

1. Access your cPanel account
2. Set up Node.js app in the Software section
3. Upload the repository files via File Manager
4. Configure environment variables
5. Start the application

Note: cPanel is not ideal for long-running Node.js applications.

### RDP (Windows)

1. Connect to your RDP
2. Install Node.js for Windows
3. Clone the repository
4. Open PowerShell and navigate to the project directory
5. Run the following commands:

```powershell
npm install
# Create .env file with required values
npm start
```

## 📝 Usage

Once the bot is running, users can interact with it on Telegram:

1. Start a chat with your bot
2. Use `/start` to get started
3. Send queries to get responses from Blackbox.ai

## ⚙️ Configuration

You can customize the bot behavior by modifying the following files:

- `config.js`: General bot configuration
- `handlers/`: Custom message handlers
- `middlewares/`: Custom middlewares

## 👨‍💻 Contributors

<a href="https://github.com/siputzx/blbx-bot/graphs/contributors">
  <img src="https://contrib.rocks/image?repo=siputzx/blbx-bot" />
</a>

Special thanks to siputzx and the BlackBox.ai team!

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the project
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgements

- [Blackbox.ai](https://www.blackbox.ai) for providing the API
- [Telegraf](https://github.com/telegraf/telegraf) for the Telegram Bot framework
- All contributors who have helped with the project

---

<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&height=100&section=footer" width="100%">
</p>
