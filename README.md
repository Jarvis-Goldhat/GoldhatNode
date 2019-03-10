# GoldhatNode
ScreenHD
# Goldhat Node 1 - Screen HD Controller  
# This node which will have a hdmi will have Kodi and Retropie installed   
# cloneable config which has all affected folders available 
# Mount Network Drive
# install curlftl to mount network drive
sudo apt-get update && sudo apt-get upgrade -y && sudo apt-get install curlftpfs -y
## Add Network Drive
mkdir /home/pi/media/ /home/pi/media/netdrive/ /home/pi/media/nasdrive
Make changes to fstab
sudo nano /etc/fstab
curlftpfs#user":"password"@"hostip".local:21/ /home/pi/media/netdrive ,fuse auto,user,uid=52,allow_other,_netdev 0 0
curlftpfs#"user":"password"@"hostip".local:21/ /home/pi/media/nasdrive ,fuse auto,user,uid=52,allow_other,_netdev 0 0

# Back up raspberry pi
sudo apt-get install deja-dup

# install virtualenv
pip install virtualenv
# Summary of Sound and Video Programmes
# Audacity
# Kodi, youtube
# Mopidy
# VLC
# retropie , with snes + street fighter, mario cart + red alert, quake, doom, wolfenstein
#### 


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
