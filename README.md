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
+ from root 
  
  ```bash
  proot-distro login --user user ubuntu-20.04
  ```
## Update & upgrade Ubuntu
```bash
sudo apt update -y && sudo apt upgrade -y
```

