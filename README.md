# fedora-games-fixes

### Dead Island Definitive Edition
### Dead Island Riptide Definitive Edition
### Dying Light
```
sudo ln -s /sbin/lspci /usr/bin/lspci
```
Borked on Fedora 35+! Game crashes silently even after resolving library issue with the below commands
```
sudo ln -s /usr/lib64/libcurl.so.4 /usr/lib64/libcurl-gnutls.so.4
dnf copr enable aflyhorse/libjpeg 
sudo dnf install libjpeg8 
```

### Mount & Blade: Warband
```
sudo ln -s /usr/lib64/libcurl.so.4 /usr/lib64/libcurl-gnutls.so.4
```
