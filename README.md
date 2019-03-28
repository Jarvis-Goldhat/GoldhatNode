# Screen Raspberry Pi - Goldhat Node 1 - 3.5 inch Screen Controller  
# Node which will have a hdmi cable into TV and separate screen  
## OS: Raspbian, Kodi media and Lakka Retrogaming installed on noobs  
Install Screen
1.)Step1, Install Raspbian 
https://www.raspberrypi.org/downloads/
b)Use“etcher”to Format your TF Card

2.) Step2, Clone my repo onto your pi
Use SSH to connect the raspberry pi, 
And Ensure that the raspberry pi is connected to the Internet before executing the following commands:
sudo rm -rf LCD-show
git clone https://github.com/goodtft/LCD-show.git
chmod -R 755 LCD-show
cd LCD-show/

3.)Step3, According to your LCD's type, excute:
In case of 3.5inch RPi Display(MPI3501)
sudo ./LCD35-show

In case of 3.5" HDMI Display-B(MPI3508)
sudo ./MPI3508-show

In case of 3.5" High Speed display(MHS35)
sudo ./MHS35-show


In case of 7inch HDMI Display-B-800X480(MPI7001)
sudo ./LCD7B-show

In case of 7inch HDMI Display-C-1024X600(MPI7002)
sudo ./LCD7C-show


If you need to switch back to the traditional HDMI display
sudo ./LCD-hdmi

Wait a few minutes,the system will restart automaticall , enjoy with your LCD.
The LCD-show.tar.gz also can be download from: http://www.lcdwiki.com/RaspberryPi-LCD-Driver 
# Summary of 3.5 Screen Install
sudo rm -rf LCD-show && git clone https://github.com/goodtft/LCD-show.git && chmod -R 755 LCD-show && cd LCD-show/ && sudo ./LCD35-show
# switch back to the traditional HDMI display
sudo ./LCD-hdmi


# Mount Network Drive
# Update &  to mount network drive (install curlftl)
sudo apt-get update && sudo apt-get upgrade -y && sudo apt-get install curlftpfs -y
mkdir /home/pi/media/ /home/pi/media/netdrive/ /home/pi/media/nasdrive
# add changes to fstab for autoboot
sudo nano /etc/fstab
curlftpfs#user":"password"@"hostip".local:21/ /home/pi/media/netdrive ,fuse auto,user,uid=52,allow_other,_netdev 0 0
curlftpfs#"user":"password"@"hostip".local:21/ /home/pi/media/nasdrive ,fuse auto,user,uid=52,allow_other,_netdev 0 0

# Back up raspberry pi
sudo apt-get install deja-dup
sudo mkdir /home/pi/media/nasdrive/Backup/Pis/ScreenPi1/
sudo mkdir /home/pi/media/nasdrive/Backup/Pis/ScreenPi2/
sudo mkdir /home/pi/media/nasdrive/Backup/Pis/ScreenPi3/
sudo mkdir /home/pi/media/nasdrive/Backup/Pis/ScreenPi7/
sudo mkdir /home/pi/media/nasdrive/Backup/Pis/GoogleAiYDancingSpeaker1/
sudo mkdir /home/pi/media/nasdrive/Backup/Pis/GoogleAiYDancingSpeaker2/
sudo mkdir /home/pi/media/nasdrive/Backup/Pis/GoogleAIYMiniSpeaker/
sudo mkdir /home/pi/media/nasdrive/Backup/Pis/GoogleAIYMiniSpeaker/

# install virtualenv
pip install virtualenv virtualenvwrapper
# Before you continue, add some lines to the ~/.bashrc  profile. Open the file using nano , vim , or emacs  and append these lines to the end:
sudo nano ~/.bashrc 
# virtualenv and virtualenvwrapper
export WORKON_HOME=$HOME/.virtualenvs
export VIRTUALENVWRAPPER_PYTHON=/usr/bin/python3
source /usr/local/bin/virtualenvwrapper.sh
# folder structure
mkdir projects projects/voice projects/vision projects/scrapy projects/websites projects/screens octapi printing games retropie lakka
 # nodes projects
  # sound
   # voice
   # Audacity
   # Mopidy
   # VLC
  # vision
  # scrapy
  # websites
  # screens 
  # octapi
  # printing
  # games
   # retropie
   # lakka
   # Kodi, youtube
   # retropie , with snes + street fighter, mario cart + red alert, quake, doom, wolfenstein

# Summary of Sound and Video Programmes
# Kodi with Network access, youtube 

# Retropie with snes mario cart 

#

Goldhat Node 
Screen 1
# this node will have vlc, google aiy, lamp, 

Stack 1 x 4
1 Pan and tilt and voice capture
2 x 2 Video capture 
> Using motioneye
>>> timelapse
>>> motion detection


2 x Voice capture


Using motioneye

Film studio
# cloneable config which has all affected folders available 
