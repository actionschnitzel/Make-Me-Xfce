# :goberserk:/// Make-Me-Xfce /// For RaspberryPi OS ///:goberserk:
    
    
![GUI](https://github.com/actionschnitzel/tingsandstuff/blob/main/github-xfce.png)

# :goberserk: PiGro Method
    
If you don't wanna walk throu the terminal jungle use the "LOOK-TAB" in PiGro
```sh
git clone https://github.com/actionschnitzel/PiGro-Aid-.git
cd PiGro-Aid-
sudo chmod +x install.sh
sudo ./install.sh
```
    
1.In Look click Tasksel    
>select Xfce > press "Tab" > press "ENTER" 
      
2.In Look click Change Desktop
>select "Nr." of "/usr/bin/startxfce4" > press "ENTER"
  
3.In Look click Change Win-Manager
> select "Nr." of "/usr/bin/xfwm4" > press "ENTER"
    
3.In Look click Wifi-Fix

Done! > REBOOT double DONE!

Xfce themes
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
    
## :pencil2:Purge-PIXEL
    
Attention! these lines remove all Raspi standard desktop components. You don't need to execute 'em.
```sh    
sudo apt remove lxde* --purge -y
    
sudo apt remove pipanel --purge -y 
    
sudo apt remove lxpanel --purge -y 
    
sudo apt remove openbox* --purge -y
    
sudo apt remove obconf --purge -y
    
sudo apt autoremove -y    
    
sudo reboot    
    
#DONE!
```
## Bonus: Don't forget Wiskermenu ;-)
