# Screen Raspberry Pi - Goldhat Node 1 - 3.5 inch Screen Controller  
# Node which will have a hdmi cable into TV and separate screen  
## OS: Raspbian, Kodi media and Lakka Retrogaming installed on noobs  
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
/home/pi/media/nasdrive/Backup/Pis/ScreenPi/

# install virtualenv
pip install virtualenv
source 
# folder structure
mkdir voice vision scrapy websites screens octapi printing games retropie lakka
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
