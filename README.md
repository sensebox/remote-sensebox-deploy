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
- 🛫 Run `docker-compose up -d`

### Setup Restreamer
- ⚙️ Open https://remote-sensebox-stream.loca.lt/ and login
- 🎞 Create the stream as descibed here: https://datarhei.github.io/restreamer/docs/guides-raspicam.html


🚀 Your remote senseBox experience should now be running on https://remote-sensebox.loca.lt/
