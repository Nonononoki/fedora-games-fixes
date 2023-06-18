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



### Dark Souls 3 Randomizer

Install the Randomizer:

To run the Randomizer .exe in the same prefix, add it as a Steam game and add the following Launch Options:
```
STEAM_COMPAT_DATA_PATH="~/.steam/steam/steamapps/compatdata/374320" %command%
```
You will need an older version of the DS3 executable:
https://drive.google.com/file/d/1nzP0SjRDex6RWrk2ntUv04N150toKQSX/view

Finally, add the following Launch Options to the main game:
```
WINEDLLOVERRIDES="dinput8.dll=n,b" %command%
```
