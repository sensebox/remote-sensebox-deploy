# 🔭 Remote senseBox deployment

### Setup Raspberry Pi
- 💾 Install Raspbian OS on your Raspberry Pi SD Card
- 🐳 You may need to install `git` and `docker` / `docker-compose`
- 📽 Enable Camera trough `sudo raspi-config`
- 🔌 Connect senseBox MCU with a USB port

### Setup Repository
- 👯 Clone this repo
- 📥 Add submodules (if needed)
- 👩‍🔧 Run `bash init.sh`
- 🛫 Run `docker-compose up -d app jsonserver restreamer localtunnel-restreamer`

### Setup API
- 🖥 Install PM2 with `npm install pm2 -g`
- 🗂 `cd backend`
- 🌳 Change .env if needed
- 🚀 `pm2 start server/index.js`
- 🗂 `cd ..`

### Start NGINX
- 🌐 `docker-compose up -d nginx localtunnel`

### Setup Restreamer
- ⚙️ Open https://remote-sensebox-stream.loca.lt/ and login
- 🎞 ~~Create the stream as descibed here: https://datarhei.github.io/restreamer/docs/guides-raspicam.html~~ Create a twitch stream

### TODO
- Twitch Stream Embedding
- HTTP Tunnel (e.g. pitunnel)

🚀 Your remote senseBox experience should now be running on https://remote-sensebox.loca.lt/
