start
```
printf '%s %s\n%s %s\n' 'nameserver' '8.8.8.8' 'nameserver' '8.8.4.4' > /etc/resolv.conf
sed -i 's/main/main contrib non-free/g' /etc/apt/sources.list
apt-get update
apt-get install firmware-amd-graphics firmware-realtek libgl1-mesa-dri libglx-mesa0 mesa-vulkan-drivers xserver-xorg-video-amdgpu
```
reboot
```
apt-get install xserver-xorg-core xserver-xorg-input-all xinit --no-install-suggests --no-install-recommends
```

```
apt-get install lightdm --no-install-suggests --no-install-recommends
```
```
apt-get install xfce4 --no-install-suggests --no-install-recommends
apt-get install xfce4-terminal --no-install-suggests --no-install-recommends
```
