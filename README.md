# 🔭 Remote senseBox deployment

### Setup Raspberry Pi
- 💾 Install Raspbian OS on your Raspberry Pi SD Card
- 🐳 You may need to install `git` and `docker` / `docker-compose`
- 📽 Enable Camera trough `sudo raspi-config`
- 🔌 Connect senseBox MCU with a USB port

### Setup Pitunnel
- https://www.pitunnel.com/

### Setup Repository
- 👯 Clone this repo
- 📥 Add submodules (if needed)
- 👩‍🔧 Run `bash init.sh`

### Setup Restreamer
- 🛫 Run `docker-compose up -d restreamer localtunnel-restreamer`
- ⚙️ Open https://remote-sensebox-stream.loca.lt/ and login
- 🎞 Create a twitch stream: https://datarhei.github.io/restreamer/docs/guides-twitch.html

### Setup Frontend
- Insert correct Twitch Link with desired Hostname in frontend/.env file
- 🛫 Run `docker-compose up -d app jsonserver`

### Setup API
- 🖥 Install PM2 with `npm install pm2 -g`
- 🗂 `cd backend`
- 🌳 Change .env if needed
- 🚀 `pm2 start server/index.js`
- 🗂 `cd ..`

### Start NGINX
- 🌐 `docker-compose up -d nginx localtunnel`

🚀 Your remote senseBox experience should now be running on https://remote-sensebox.loca.lt/
