# pi_video_looper
Application to turn your Raspberry Pi into a dedicated looping video playback device, good for art installations, information displays, or just playing cat videos all day.

Video_looper guide: https://learn.adafruit.com/raspberry-pi-video-looper?view=all
Configuration of Pi: https://www.raspberrypi.org/documentation/configuration/

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

## Change time-interval for volume-ON
In file: Adafruit_Video_Looper/video_looper.py change the variables on line 71-72
```
_START_TIME = "08:00"
_END_TIME = "20:00"
```
