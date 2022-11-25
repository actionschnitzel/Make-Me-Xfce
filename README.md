# :goberserk:/// Make-Me-Xfce /// For RaspberryPi OS ///:goberserk:

>https://www.xfce-look.org/browse/    
    
# :goberserk: Terminal Method
    
## :pencil2:Prepaire for Xfce4
```sh
sudo apt-get update -y

sudo apt install xfce4 xfce4-terminal xfce4-goodies -y
```

## :pencil2:Change Desktop

```sh
sudo update-alternatives --config x-session-manager
```
>/usr/bin/startxfce4 # to select
    
```sh
sudo update-alternatives --config x-window-manager
```    
>/usr/bin/xfwm4      # to select
    
```sh
sudo reboot
```    
    
## :pencil2:Wifi-FIX
    
For some reason Wifi isn't working with the standard manager    
```sh
sudo apt install network-manager-gnome -y                
   
sudo systemctl disable dhcpcd
    
sudo /etc/init.d/dhcpcd stop
    
sudo reboot
```    


## :pencil2:Bluetooth-FIX
    
If bluetooth isn't working    
```sh
sudo apt install bluetooth pulseaudio-module-bluetooth blueman bluez-firmware
    
sudo reboot
```   

## :pencil2:Password-Prompt-FIX
```sh
sudo apt install gnome-keyring libpam-gnome-keyring 
    
sudo reboot
```  
## :pencil2:Good Theme
```sh
sudo apt install numix-gtk-theme
    
sudo reboot
```  

## Bonus: Don't forget Wiskermenu ;-)
