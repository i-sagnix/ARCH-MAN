# yay
    full system update
        yay -Syu    OR,    yay
    install pkg
        yay -S <pkg_name>
    search pkg
        yay -Ss <pkg_name>
    search then install pkg
        yay -ss <pkg_name>      OR,
        yay <pkg_name>
    remove pkg
        yay -R <pkg_name>    
    remove pkg & dependencies(if not used by others)
        yay -Rns <pkg_name>
        5:16 PM
    clear cache
        yay -Sc    
    list explicitly installed packages
        yay -Qe

abbreviation list-commands
    ..  ='cd ..'
    ... ='cd ../..'
    mk  ="mkdir -p"`    #mkdir with parent folders if non existant
    gic ='git clone'

whoami         #display username
hostnamectl    #display hostname
findmnt        #list and search for file systems
lsblk / lsblk -t #list partition block devices

change file permissions
    chmod -R 700 file/directory_path
      (R=recursive) (700 = u(user)g(group)o(other) octal rwx value where r=octal(100)=4 w=2 x=1)     

chown -R     #change ownership

systemctl enable adn start combined
    systemctl enable --now #service_name

cli-network-tools
    ip a //show ip info  ,     ip //for help

To check swap status, use:
$ swapon --show

Or to show physical memory as wxell as swap usage:
$ free -h

sysctl
    To load all configuration files manually, execute:
    # sysctl --system 
    A single parameter file can also be loaded explicitly with:
    # sysctl --load=filename.confw

fontconfig
    To see a list of known Fontconfig fonts:
    $ fc-list ':' file
    
wpctl    wireplumber control

sudo -v    (Refresh the sudo timeout)
sudo -K    (Revoke sudo)


#HYPRPM (hyprland plugins)
enable or disable them via hyprpm enable name and hyprpm disable name.
In order for the plugins to be loaded into hyprland, run hyprpm reload.
You can add    exec-once = hyprpm reload -n    to your hyprland config to have plugins loaded at startup. -n will make hyprpm send a notification if anything goes wrong (e.g. update needed)
For all options of hyprpm, run hyprpm -h.


SYS-INFO / SYS-MONITOR
    neofetch
    cpufetch
    btop

FUN
    cava
    cmatrix
    COOL RETRO TERMINAL

NVME/SATA SSD
    smartctl
        sudo smartctl --info /dev/... , smartctl --all /dev/...

root privileges in nautilus
    Ctrl + L, admin://

    convert -list font | less     #to obtain a list of fonts available on your computer

KITTY TERMINAL
    kitten @ --help    #To get a list of available actions, in kitty
    kitty +list-fonts  #To list fonts
    
