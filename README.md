# Remote senseBox deployment

## Installation
### Setup Raspberry Pi
- Install Raspbian OS on your Raspberry Pi SD Card
- You may need to install `git` and `docker / docker-compose`
- Enable Camera trough `sudo raspi-config`

### Setup Repository
- clone this repo
- add submodules
- move Dockerfile to backend
- run `docker-compose up -d`

### Setup Restreamer
- Open https://remote-sensebox-stream.loca.lt/ and login
- Create the stream as descibed here: https://datarhei.github.io/restreamer/docs/guides-raspicam.html

### Setup Frontend
- Start the Frontend on netlify with the corresponding environment variables