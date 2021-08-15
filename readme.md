
   ██╗░░░░░███╗░░░███╗███╗░░██╗████████╗██████╗░░░███╗░░██╗░░██╗
   ██║░░░░░████╗░████║████╗░██║╚══██╔══╝██╔══██╗░████║░░╚██╗██╔╝
   ██║░░░░░██╔████╔██║██╔██╗██║░░░██║░░░██████╔╝██╔██║░░░╚███╔╝░
   ██║░░░░░██║╚██╔╝██║██║╚████║░░░██║░░░██╔══██╗╚═╝██║░░░██╔██╗░
   ███████╗██║░╚═╝░██║██║░╚███║░░░██║░░░██║░░██║███████╗██╔╝╚██╗
   ╚══════╝╚═╝░░░░░╚═╝╚═╝░░╚══╝░░░╚═╝░░░╚═╝░░╚═╝╚══════╝╚═╝░░╚═╝

#### LoneRiced

These are the configurations tested in Kali-linux (virtualized), It is also scalable in other distributions. The main checkpoints are present in the git dependencies. If you want, try it.


###### Nota
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
**A quick guide regardless  [Here](https://github.com/VaughnValle/blue-sky)**



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
###### Nota:  
We use Firejail to encapsulate Firefox as the first security rule, other programs can also be encapsulated according to your needs. Otherwise you can skip this step and you will have to edit the file `.config/sxhkd/sxhkdrc`

    #Open Firefox
    super + shift + f
            firejail /opt/firefox/firefox      // It should change only by " Firefox "
    
    
### Instalación Automática

In this way we install the script  `install.sh`


### Instalación Manual
** I. Copy all files to `$HOME/.config/`: **
  
- bspwm
- polybar
- rofi
- sxhkd
- picom

**II. Copiamos la carpeta` .fonts` en `$home/`**

### Cambiar de Thema a Rofi
To change the theme to rofi you just need to execute this line in a terminal

    $
    $Rofi-theme-selector
    $
	
Next we move until we find the option `NORD ` and then with` Alt  +  A` save the configuration.

    
###Images

Desktop:

![](https://i.imgur.com/CXz62q9.png)

Rofi:

![](https://i.imgur.com/mftDzfD.png)




