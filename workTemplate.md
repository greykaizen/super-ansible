- target OS
    - dnf(fedora)
    - apt(ubuntu, popos)
    - pacman(arch, cachyos)


- pre-tasks
    - update repos
    - update system
    - 
- target tasks
    - 🟢pkgs
        - gcc make jq jre21-openjdk-headless
        libplasma kauth podman docker git zoxide fzf bat fish
        tmux aria2 fastfetch alacritty distrobox gnome-boxes
        vlc libreoffice-fresh okular qalculate-qt qbittorrent
        kile kate kwrite gwenview
        "kio-admin" chezmoi openssh rustup zed
    - 🟢flatpaks
        - - com.brave.Browser
        - app.zen_browser.zen
        - io.github.dvlv.boxbuddyrs
        - org.jousse.vincent.Pomodorolm
        - org.telegram.desktop
        - com.github.tchx84.Flatseal
    - 🟢aur helper installation
        - "mediawriter"
        - "visual-studio-code-bin"
        - "thorium-browser-bin"
    - 🟢fonts
        - https://github.com/ryanoasis/nerd-fonts/releases/download/v3.3.0/CascadiaCode.zip
        - https://github.com/ryanoasis/nerd-fonts/releases/download/v3.3.0/FiraCode.zip
        - https://github.com/ryanoasis/nerd-fonts/releases/download/v3.3.0/JetBrainsMono.zip
        - https://github.com/ryanoasis/nerd-fonts/releases/download/v3.3.0/Meslo.zip
        - https://github.com/ryanoasis/nerd-fonts/releases/download/v3.3.0/Noto.zip
        - https://github.com/ryanoasis/nerd-fonts/releases/download/v3.3.0/RobotoMono.zip
        - https://github.com/ryanoasis/nerd-fonts/releases/download/v3.3.0/Ubuntu.zip
    - 🟢icons
        - https://github.com/ful1e5/Bibata_Cursor/releases/download/v2.0.7/Bibata-Modern-Classic.tar.xz
        - https://github.com/ful1e5/Bibata_Cursor/releases/download/v2.0.7/Bibata-Modern-Ice.tar.xz
    - 🟢grub
        - install os-prober, run it
        - sudo grub-mkconfig -o /boot/grub/grub.cfg
    - 🟢plymouth
        - plymouth-set-default-theme -R spinner
    - 🟢grub wallpaper
        - cp /wallpaper/splash.png /usr/share/wallpapers/cachyos-wallpapers/splash.png

- additional
    - file split
    - tasks
        - systemctl
            - docker start and it's hello-world and then docker stop
        - rustup
            - rustup default stable
            - some check like cargo new project in ~/Projects and if it's successful, delete the project (opt)
        - chezmoi (install and run)
            - PAT require for git
            - init --apply -v
        - shell setup
            - clone configs-cachyos and install fish, zsh (plugins as well)
            - default shell setup
            - shell profile
    - OS
        - fedora
        - Ubuntu, popos
        
- structure refine
.
├── ansible.cfg
├── arch
│   ├── aur_pkg.yml
│   ├── extra.yml
│   ├── flatpaks.yml
│   ├── fonts.yml
│   ├── icons.yml
│   ├── in_aur_pkg.yml
│   ├── in_flatpaks.yml
│   ├── in_font_icons.yml
│   ├── in_pkg.yml
│   ├── packages.yml
│   └── wallpaper
│       └── splash.png
├── inventory

- todo
    
- progress
    - marked as 🟢
