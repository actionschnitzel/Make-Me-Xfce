# :goberserk:/// Make-Me-Xfce /// 4 RaspberryPi OS ///:goberserk:
    
    
![GUI](https://github.com/actionschnitzel/tingsandstuff/blob/main/github-xfce.png)

    
## :pencil2:Prepaire for Xfce4

>sudo apt-get update -y

>sudo apt install xfce4 xfce4-terminal xfce4-goodies -y


## :pencil2:Change Desktop

>sudo update-alternatives --config x-session-manager

>/usr/bin/startxfce4
    
>sudo update-alternatives --config x-window-manager
    
>/usr/bin/xfwm4
    
>sudo reboot
    
    
## :pencil2:Wifi-FIX
    
For some reason Wifi isn't working with the standard manager    
>sudo apt install network-manager-gnome -y                
    
>sudo systemctl disable dhcpcd
    
>sudo /etc/init.d/dhcpcd stop
    
>reboot
    
    
## :pencil2:Purge-PIXEL
    
Attention! these lines remove all Raspi standard desktop components. You don't need to execute 'em.
    
>sudo apt remove lxde* --purge -y
    
>sudo apt remove pipanel --purge -y 
    
>sudo apt remove lxpanel --purge -y 
    
>sudo apt remove openbox* --purge -y
    
>sudo apt remove obconf --purge -y
    
>sudo apt autoremove -y    
    
>sudo reboot    
    
#DONE!

## Bonus: Dont't forget Wiskermenu ;-)
