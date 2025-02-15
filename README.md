# 🤖 Blackbox.ai Telegram Bot

![Blackbox.ai Telegram Bot](https://socialify.git.ci/siputzx/blbx-bot/image?description=1&descriptionEditable=Integrate%20Blackbox.ai%20API%20with%20Telegram%20Bot&font=Inter&forks=1&issues=1&language=1&name=1&owner=1&pattern=Circuit%20Board&pulls=1&stargazers=1&theme=Dark)

<div align="center">
  
  [![GitHub stars](https://img.shields.io/github/stars/siputzx/blbx-bot?style=for-the-badge&color=gold)](https://github.com/siputzx/blbx-bot/stargazers)
  [![GitHub forks](https://img.shields.io/github/forks/siputzx/blbx-bot?style=for-the-badge&color=blue)](https://github.com/siputzx/blbx-bot/network/members)
  [![GitHub issues](https://img.shields.io/github/issues/siputzx/blbx-bot?style=for-the-badge&color=red)](https://github.com/siputzx/blbx-bot/issues)
  [![GitHub license](https://img.shields.io/github/license/siputzx/blbx-bot?style=for-the-badge&color=green)](https://github.com/siputzx/blbx-bot/blob/main/LICENSE)
  
  <a href="https://github.com/siputzx/blbx-bot">
    <img src="https://api.visitorbadge.io/api/visitors?path=siputzx.blbx-bot&label=VISITORS&labelColor=%23007EC6&countColor=%23263759" alt="Visitors Badge"/>
  </a>
  
</div>

<p align="center">
  <img src="https://img.shields.io/badge/Node.js-43853D?style=for-the-badge&logo=node.js&logoColor=white" alt="Node.js">
  <img src="https://img.shields.io/badge/Telegram-2CA5E0?style=for-the-badge&logo=telegram&logoColor=white" alt="Telegram">
  <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black" alt="JavaScript">
</p>

## 📊 Project Stats

<div align="center">
  
  ![GitHub repo size](https://img.shields.io/github/repo-size/siputzx/blbx-bot?style=for-the-badge&color=blueviolet)
  ![GitHub last commit](https://img.shields.io/github/last-commit/siputzx/blbx-bot?style=for-the-badge&color=purple)
  ![GitHub contributors](https://img.shields.io/github/contributors/siputzx/blbx-bot?style=for-the-badge&color=teal)
  
</div>

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api/pin/?username=siputzx&repo=blbx-bot&theme=radical" alt="Repo Card"/>
</p>

## ✨ Features

- 🚀 Seamless integration of Blackbox.ai API with Telegram
- ⚡ Lightning-fast responses to user queries
- 💻 Advanced code generation and assistance
- 🌍 Multi-platform deployment support
- 🧠 Intelligent conversation handling
- 🛠️ Minimal resource requirements
- 🎨 Modern and elegant interface

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

<details>
<summary><b>📱 Termux (Android)</b></summary>
<br>

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

3. To keep the bot running after closing Termux, install `tmux`:

```bash
pkg install tmux
tmux new -s bot
# Run your bot inside this session
# To detach: press Ctrl+b, then d
# To reattach: tmux attach -t bot
```
</details>

<details>
<summary><b>☁️ Replit</b></summary>
<br>

1. Create a new Replit project
2. Import from GitHub: `https://github.com/siputzx/blbx-bot.git`
3. Add secrets in Replit for `BOT_TOKEN` and `BLACKBOX_API_KEY`
4. Create a file called `.replit` with:

```
language = "nodejs"
run = "npm start"
```

5. Click Run button
6. Use UptimeRobot to ping your Replit URL to keep it alive
</details>

<details>
<summary><b>🚀 Heroku</b></summary>
<br>

1. Create a Heroku account and install Heroku CLI
2. Clone the repository locally
3. Create a `Procfile` with:

```
worker: npm start
```

4. Initialize Heroku app:

```bash
heroku login
heroku create your-app-name
git push heroku main
heroku config:set BOT_TOKEN=your_telegram_bot_token
heroku config:set BLACKBOX_API_KEY=your_blackbox_api_key
heroku ps:scale worker=1
```
</details>

<details>
<summary><b>🦖 Pterodactyl Panel</b></summary>
<br>

1. Create a new Node.js server in your panel
2. Set startup command to `npm start`
3. Upload the repository files
4. Add environment variables in the Startup tab:
   - `BOT_TOKEN`
   - `BLACKBOX_API_KEY`
5. Start the server
</details>

<details>
<summary><b>🖧 VPS (Ubuntu/Debian)</b></summary>
<br>

1. Connect to your VPS via SSH
2. Install Node.js and npm:

```bash
sudo apt update
sudo apt install nodejs npm
git clone https://github.com/siputzx/blbx-bot.git
cd blbx-bot
npm install
```

3. Create a systemd service for auto-restart:

```bash
sudo nano /etc/systemd/system/blbx-bot.service
```

4. Add the following content:

```
[Unit]
Description=Blackbox.ai Telegram Bot
After=network.target

[Service]
Type=simple
User=your_username
WorkingDirectory=/path/to/blbx-bot
ExecStart=/usr/bin/npm start
Restart=on-failure
Environment=BOT_TOKEN=your_telegram_bot_token
Environment=BLACKBOX_API_KEY=your_blackbox_api_key

[Install]
WantedBy=multi-user.target
```

5. Enable and start the service:

```bash
sudo systemctl enable blbx-bot
sudo systemctl start blbx-bot
```
</details>

<details>
<summary><b>☁️ Koyeb</b></summary>
<br>

1. Sign up for a Koyeb account
2. Connect your GitHub account
3. Create a new app from the GitHub repository
4. Add environment variables:
   - `BOT_TOKEN`
   - `BLACKBOX_API_KEY`
5. Set the run command to `npm start`
6. Deploy the application
</details>

<details>
<summary><b>🌐 cPanel (Not Recommended)</b></summary>
<br>

1. Access your cPanel account
2. Set up Node.js app in the Software section
3. Upload the repository files via File Manager
4. Create `.env` file with required values
5. Configure application to run as a service:
   - Use Setup Node.js App feature
   - Set entry point to `index.js`
   - Enable application autorestart
   
Note: cPanel is not ideal for long-running Node.js applications as it may have limitations on process runtime.
</details>

<details>
<summary><b>🖥️ RDP (Windows)</b></summary>
<br>

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

6. To run as a Windows service, install pm2:

```powershell
npm install -g pm2
pm2 start index.js --name "blbx-bot"
pm2 startup
pm2 save
```
</details>

## 📝 Usage

<div align="center">
  <img src="https://i.ibb.co/Qf79bVQ/telegram-bot-demo.png" alt="Bot Demo" width="300px"/>
</div>

Once the bot is running, users can interact with it on Telegram:

1. Start a chat with your bot
2. Use `/start` to get started
3. Send queries to get responses from Blackbox.ai
4. Available commands:
   - `/help` - Show help message
   - `/status` - Check bot status
   - `/reset` - Reset conversation
   - `/settings` - Configure user preferences

## ⚙️ Configuration Options

You can customize the bot behavior by modifying the following files:

- `config.js`: General bot configuration
- `handlers/`: Custom message handlers
- `middlewares/`: Custom middlewares

Advanced configuration options:
```javascript
{
  "responseDelay": 500,       // Delay in ms before responding
  "maxConversationLength": 10, // Maximum conversation history to maintain
  "blackboxModel": "default",  // AI model to use
  "debugMode": false,         // Enable verbose logging
  "rateLimiting": {
    "maxRequests": 30,        // Maximum requests per window
    "window": 60              // Time window in seconds
  }
}
```

## 📊 Usage Analytics

<div align="center">
  <img src="https://quickchart.io/chart?c={type:'line',data:{labels:['Jan','Feb','Mar','Apr','May','Jun'],datasets:[{label:'Users',data:[120,150,180,220,270,300],borderColor:'rgb(75,192,192)',tension:0.1}]}}" alt="User Growth Chart"/>
</div>

## 👨‍💻 Contributors

<a href="https://github.com/siputzx/blbx-bot/graphs/contributors">
  <img src="https://contrib.rocks/image?repo=siputzx/blbx-bot" />
</a>

Special thanks to siputzx and the BlackBox.ai team for their incredible contributions!

## 🌟 Stargazers Over Time

<div align="center">
  <a href="https://star-history.com/#siputzx/blbx-bot&Date">
    <img src="https://api.star-history.com/svg?repos=siputzx/blbx-bot&type=Date" alt="Star History Chart">
  </a>
</div>

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

<div align="center">
  
  <img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&height=100&section=footer&text=Made%20with%20%E2%9D%A4%EF%B8%8F%20by%20siputzx&fontSize=24&fontAlignY=80" width="100%">
  
</div>
