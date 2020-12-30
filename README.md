# 2021_rpi_linux
ManjaroARM Linux for my Raspberry Pis

## Links

- https://manjaro.org/support/firststeps/ (See Setup for my notes on this)
- https://wiki.manjaro.org/
- https://forum.manjaro.org/
- https://github.com/swaywm/sway modern Wayland based Window Manager (i3 compatible)

## Setup

### First Setup (RaspberryPi3 - 2020-12-30)

- **Hardware:**
  - I use my LEGO housed RPi3-Stack with e-Paper Status Display and PiPower fallback
  - Connected to a keyboard and a HDMI monitor
  - I use a 32 GB micro SD-Card for now ((looking for a faster choice later))
  - My first host is a Windows 10 machine for now 
    - using balneaEtcher for image creation
- **Image:**
  - Download: https://osdn.net/projects/manjaro-arm/storage/rpi4/sway/20.10/Manjaro-ARM-sway-rpi4-20.10.img.xz/
    - size is 1.1 GB 
    - _wait_
  - Insert microSD Card via Adapter to PC in unlocked mode
  - Start balneaEtcher (select image + select drive + start )
  - _wait_ 
  - remove the car ((A nice thing with balneaEtcher is the autoremove function of the SD-card so you are free to remove it without any fuzz))
 - **First Boot, Setup and Second Boot Into Sway:**
   - follow the setup wizard
   - _wait_ setup and rebooting
   
 - **Third Boot Into Sway:**
   - Login ((user and password))
   - [Sway Cheat Sheet](https://depau.github.io/sway-cheatsheet/)
   
   - install with `sudo pacman -S {{packet}}`
     - python 3.8 is already installed
     - git 2.28 is already installed
     - vim 8.2
     - lua 5.4
     - clang 11.0
     - ruby 2.7
     - rust 1.47
     - npm 6.14.8
     - nodejs 14.13   
     - asciidoctor 2.0
   
     - {--postgresql 12.5 (for gitea)--}
     - [gitea 1.12.5](https://docs.gitea.io/en-us/command-line/)
     
   - setup gitea
     - {--`sudo systemctl enable postgresql`--}
     - {--`sudo systemctl start postgressql`--}
     - start gitea `sudo gitea web --port 3000` 
     - browse to `https://{{ip_a}}:{{port}}` 
     -
   
## maybe later:   
   - kodi
   
## Historical

During my Christmas Holidays I choose to setup my old Raspberry Pi 3 with a working system.
After some hardware extensions work (Sunfoders PiPower and a 2.7inch e-Paper display HAT from waveshare and an extensible LEGO housing) I was ready for the first thoughest question on a Linux system: "Which distribution to use". 

My goal was a system that would be usable in dial mode: manly from the command line but also in a GUI on device.
In a mini-server-setup I want to use HTTP and SSH access which both are pretty backed into all systems.

After some testing and probing I decided to move to the ArchLinux domain and started with the ManJaroARM project.

This seems to be the **new Ubuntu** in that domain adding some nice managers on top of the great ArchLinux system (`pacman`).

The driver manager in Manjaro seems to give me as a not to extensive Linux user a nice addition to get faster to the actual problem.

I also chose Manjoran on basis of the Forum and WIKI pages - not content only visual appearances - content and community will be tested afterwards but I am sure that both systems are powered by very great communities.

## Opinionated

My first 
