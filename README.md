# Fedora Workstation Setup
"${HOME}" sweet "${HOME}"

```
# Part 0: Prepare
sudo su
sudo echo -e "max_parallel_downloads=10\nfastestmirror=true" >> /etc/dnf/dnf.conf
sudo sh -c 'fwupdmgr refresh --force && fwupdmgr update --assume-yes'

mkdir dev/
cd dev
git clone --depth=1 --branch=main https://github.com/sotsugov/fbox.git && cd fbox
sudo bash sysprep 
sudo bash software
```
