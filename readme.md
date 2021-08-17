
   ██╗░░░░░███╗░░░███╗███╗░░██╗████████╗██████╗░░░███╗░░██╗░░██╗
   ██║░░░░░████╗░████║████╗░██║╚══██╔══╝██╔══██╗░████║░░╚██╗██╔╝
   ██║░░░░░██╔████╔██║██╔██╗██║░░░██║░░░██████╔╝██╔██║░░░╚███╔╝░
   ██║░░░░░██║╚██╔╝██║██║╚████║░░░██║░░░██╔══██╗╚═╝██║░░░██╔██╗░
   ███████╗██║░╚═╝░██║██║░╚███║░░░██║░░░██║░░██║███████╗██╔╝╚██╗
   ╚══════╝╚═╝░░░░░╚═╝╚═╝░░╚══╝░░░╚═╝░░░╚═╝░░╚═╝╚══════╝╚═╝░░╚═╝

#### LoneRiced

This environment is made in [BSPWM](https://wiki.archlinux.org/title/Bspwm_(Espa%C3%B1ol)) which is a tiled window manager, the main feature is that it presents the windows as sheets of a binary file.

These are the configurations tested on Kali-linux (virtualized), it is also scalable on other distributions. The main checkpoints are present in the git dependencies. The sources are open source, you can try it out at your own leisure.


###### Note:
- All the points and configurations are customizable, according to this installation it has been compiled from different internet sources.

#### 📝 Dependencies

Program | Name
---|---
Window Manger | [bspwm](https://github.com/baskerville/bspwm.git)
Bar | [polybar](https://github.com/polybar/polybar)
Launcher | [rofi](https://github.com/davatorium/rofi)
Wallpaper Setter | [feh](https://feh.finalrewind.org/)
Web Browser | [firefox](https://www.mozilla.org/en-US/firefox/new/)
Executing commands | [sxhkd](https://github.com/baskerville/sxhkd)
Display | [Picom](https://github.com/ibhagwan/picom)
File Manager | [thunar](https://wiki.debian.org/Thunar) or Dolphin
Shell | [gnome-terminal](https://help.gnome.org/users/gnome-terminal/stable/)
Code Editor | [neovim](https://neovim.io)
Fetch | [neofetch](https://github.com/dylanaraps/neofetch)
Telegram | [Telegram-Desktop](https://blog.desdelinux.net/como-instalar-telegram-en-linux/) (optional)
Encapsulator| [firejail](https://github.com/netblue30/firejail)

We suggest reviewing the settings and selecting what you need. These dependencies can take time but will be necessary to enjoy this environment.
**A quick guide  [Here](https://github.com/VaughnValle/blue-sky)**



------------


##  Little Installation Guide 

##### You must previously Install a new [Firefox](https://www.mozilla.org/en-US/firefox/linux/) 
 Before unpacking firefox we open a terminal and become superusers `# ` then we head to the root `#cd /  ` to later be able to assign as owner and group to your $`User` (lmntr1x) in the directory where third-party programs are hosted in this case `/opt/` :
```shell
#chown lmntr1x:lmntr1x opt/

#su  lmntr1x

$cd opt/ 

mv /home/lmntr1x/descargas/firefox-89.tar.bz2 .   
```
Once the package is extracted we will be ready for the next step.
###### Note:  
We use Firejail to encapsulate Firefox as the first security rule, other programs can also be encapsulated according to your needs. Otherwise you can skip this step and you will have to edit the file `.config/sxhkd/sxhkdrc`

    #Open Firefox
    super + shift + f
            firejail /opt/firefox/firefox      // It should change only by " Firefox "
    
    
### Automatic installation

 Before taking this step we must give administrator permissions to these files
- install.sh
- /bin/ethernet_status.sh
- /bspwm/bspwmrc  && /scritps/bspwm_resize
- /polybar/launch.sh


In this way we install the script  `install.sh`


If you have problems with the bar (Incomplete or lack of icons) it is due to the lack of the font <---> You must manually copy the file `.Fonts`  to  `$HOME/`


### Manual installation
**I. Copy all files to `$HOME/.config/`:**
  
- bspwm
- polybar
- rofi
- sxhkd
- picom

**II. Copiamos la carpeta` .fonts` en `$HOME/`**

**All these steps can be performed from the default environment | In order to see the changes you must change the environment to BSPWM**


### Change Theme to Rofi
To change the theme to rofi you just need to execute this line in a terminal

    $
    $Rofi-theme-selector
    $
	
Next we move until we find the option `NORD ` and then with` Alt  +  A` save the configuration.

    
### Images

Desktop:

![](https://i.imgur.com/CXz62q9.png)

Rofi:

![](https://i.imgur.com/mftDzfD.png)




