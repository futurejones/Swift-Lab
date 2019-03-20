# A Quick Start Guide

# Setting Up Your PC
* As we will be using "Open Source Swift" and developing on the Raspberry Pi running a Linux / Debian based OS we will also use developement tools that are available on all platforms.

* You can use a PC / Laptop running macOS, Windows or Linux.

* You will need an adapter to plug a microSD card into your PC.

# Software 
## Code Editing and Remote File Access via SSH Terminal
* ### Visual Studio Code + Remote VSCode extension
[https://code.visualstudio.com/Download](https://code.visualstudio.com/Download)

## Github Access
* ### Github Desktop App
[https://desktop.github.com/](https://desktop.github.com/)

## FTP File Access
* ### CyberDuck
[https://cyberduck.io/download/](https://cyberduck.io/download/)

## Network Scanning
* ### LanScan
[https://www.iwaxx.com/lanscan/](https://www.iwaxx.com/lanscan/)

# Raspberry Pi Setup

## Raspbian OS
* ### Install the latest Raspbian Stretch Lite OS a good quality 8GB microSD card or larger.
Etcher - [https://www.balena.io/etcher](https://www.balena.io/etcher)

ApplePi-Baker - [https://www.tweaking4all.com](https://www.tweaking4all.com/software/macosx-software/macosx-apple-pi-baker/)

For headless installation to enable SSH and WiFi connection it is necessary to copy a blank ssh file and a wpa_supplicant.conf file to the "boot" section of the microSD before installing into the Raspberry Pi. Copies of these files can be found in `raspberry-pi-setup`  
Make sure you add the WiFi network and password to the wpa_supplicant.conf file.

# Swift Installation
## Swift install using `sudo apt install`
* We will be using the `swift-arm` package repository to install Swift.

* First add the package repositorys  
* For installation of swift-lite packages use :-  
[https://packagecloud.io/swift-arm/swift-lite](https://packagecloud.io/swift-arm/swift-lite)  
Add repo - `curl -s https://packagecloud.io/install/repositories/swift-arm/swift-lite/script.deb.sh | sudo bash`  
Install swift - `sudo apt install swift-lite-rpi`
* For full installation of the latest Swift release packages use :-  
[https://packagecloud.io/swift-arm/release](https://packagecloud.io/swift-arm/release)  
Add repo - `curl -s https://packagecloud.io/install/repositories/swift-arm/release/script.deb.sh | sudo bash`  
Install swift - `sudo apt install swift4`

* For full installation of the latest swift 5 dev packages use :-  
[https://packagecloud.io/swift-arm/dev-builds](https://packagecloud.io/swift-arm/dev-builds)  
Add repo - `curl -s https://packagecloud.io/install/repositories/swift-arm/dev-builds/script.deb.sh | sudo bash`  
Install swift - `sudo apt install swift5dev`  
*NOTE: swift5dev builds are only available for aarch64 Ubuntu 16.04 and 18.04 OS*

# The Swift-Lite Project
## Info about the Swift-Lite project [https://swift-lite.org/](https://swift-lite.org/)
### We will preview the Swift-Lite Raspberry Pi Edition in the workshop.

[Back](README.md)
