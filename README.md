# Fedora Workstation Setup
"${HOME}" sweet "${HOME}"

```
# Part 0: Prepare
sudo su
sudo echo -e "max_parallel_downloads=10\nfastestmirror=true" >> /etc/dnf/dnf.conf
sudo sh -c 'fwupdmgr refresh --force && fwupdmgr update --assume-yes'

# Part 1: Installation
git clone https://github.com/sotsugov/fed-home
cd fed-home
sudo bash sysprep
sudo bash software
bash themes

# Manual Part
devcmd

```
