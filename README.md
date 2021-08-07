<h1 align=center>Flutter On Android</h1>
<h1 align=center> 
  <a href=https://play.google.com/store/apps/details?id=com.termux>
    Install ►
  </a>
  /
  <a href=https://f-droid.org/packages/com.termux>
    ⇱ TermUX
  </a>
</h1>

## Update & upgrade TermUX
```bash
pkg update -y && pkg upgrade -y
```
## SetUp Storage
```bash
termux-setup-storage
```
## Install [Proot-Distro](https://github.com/termux/proot-distro)
```bash
pkg install proot-distro -y
```
## Install Ubuntu CLI 
```bash
proot-distro install ubuntu-20.04
```
## Login in Ubuntu CLI
```bash
proot-distro login ubuntu-20.04
```
## Install sudo ( root / super user )
```bash
apt update -y && apt install sudo -y
```
## Add User
```bash
adduser user
```
## Login user
+ from root 
  ```bash
  login user
  ```
## Add Permission to user
```bash
echo "user ALL=(ALL:ALL) ALL" >> /etc/sudoers
```
## Restart TermUX

## Login user
+ from TermUX 
  
  ```bash
  proot-distro login --user user ubuntu-20.04
  ```
## Update & upgrade Ubuntu
```bash
sudo apt update -y && sudo apt upgrade -y
```
## Install Flutter from git
```bash
sudo apt install git -y
cd ~
git clone https://github.com/flutter/flutter.git -b stable
cd ~
export PATH=$PATH:~/flutter/bin
which flutter dart
flutter doctor
```
## set saving projects in internal storage 
```bash
mkdir /sdcard/FlutterApps
cd /sdcard/FlutterApps
```
## Create flutter web app
```bash
cd /sdcard/FlutterApps
flutter create `web_app_name` --platforms web
```
## Configure
```bash
flutter config --enable-web
```
## Run
```json
cd /sdcard/FlutterApps/`web_app_name`/

flutter run -d web-server --web-port 8080 # [Web-Server] : http://localhost:8080
```
## How to open app
+ Open Chrome or any browser
+ type [http://localhost:8080](http://localhost:8080) in address bar and search
+ Your app getting run 

## Edit using any editor 
## and reload using 
+ Open TermUX
+ type r to reload flutter
+ type R to restart flutter
+ type q to exit flutter



