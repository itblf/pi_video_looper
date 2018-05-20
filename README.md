# pi_video_looper
Application to turn your Raspberry Pi into a dedicated looping video playback device, good for art installations, information displays, or just playing cat videos all day.

https://learn.adafruit.com/raspberry-pi-video-looper?view=all

## Installation
Update and clone repository
```
sudo apt-get update
sudo apt-get install -y git
git clone https://github.com/rpiloop/pi_video_looper.git
```

Install
```
cd pi_video_looper
sudo ./install.sh
```

Program should automatically start loading video-files from USB.

## Usage
Stop/start looper from SSH
```
sudo supervisorctl stop video_looper
```

To disable it entirely to not start on boot
```
cd pi_video_looper
sudo ./disable.sh
```
To enable again, simply run install script
```
sudo ./install.sh
```