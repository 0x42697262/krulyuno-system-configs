# krulyuno-system-configs
Personal PKGBUILD for my arch setup. This repo is not for everyone to use since I am using this repo PKGBUILD to track my changes in my arch setup.

# Dependencies
```bash
acpilight pipewire pipewire-alsa wiruplumber pipewire-jack pipewire-pulse pipewire-audio
```

`acpilight` - adjust my monitor display brighness

`pipewire` - audio latency

`rtkit` - maybe i need this... who knows

# Installation

1. Clone this repository `git clone https://github.com/KrulYuno/krulyuno-system-configs.git`
2. Install `makepkd -si krulyuno-system-configs`

# Do these after installation
Run `post_install.sh` as root or manually run each commands:

### Making acpilight work
1. `usermod -aG video birb`


