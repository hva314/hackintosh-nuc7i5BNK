Hackintosh Catalina 10.15.7 (19H1217)

NUC7i5BNK
## Spec:
* Intel Core i5 7260U 2.20Ghz Kaby Lake 
* Intel Iris Plus Graphic 640
* ALC283

Ref: 
https://dortania.github.io/OpenCore-Install-Guide/
https://github.com/corpnewt/MountEFI
https://github.com/corpnewt/ProperTree
https://github.com/corpnewt/GenSMBIOS
https://opencore.slowgeek.com/
https://github.com/headkaze/Hackintool/releases

# Create boot USB on MAC
Download Mac Installer
```
mkdir ~/macOS-installer && cd ~/macOS-installer && curl -O https://raw.githubusercontent.com/munki/macadmin-scripts/main/installinstallmacos.py && sudo python installinstallmacos.py
```

Format USB use use macOS Extended (HFS+) with a GUID partition map

```
sudo /Applications/Install\ macOS\ Big\ Sur.app/Contents/Resources/createinstallmedia --volume /Volumes/MyVolume
```

Mount EFI partition with MountEFI

Setting up core files
https://dortania.github.io/OpenCore-Install-Guide/installer-guide/opencore-efi.html

Gathering files
https://dortania.github.io/OpenCore-Install-Guide/ktext.html#kexts

Configuring plist for Kaby Lake
https://dortania.github.io/OpenCore-Install-Guide/config.plist/kaby-lake.html#starting-point

Sanity check
https://opencore.slowgeek.com/

Post-installation 
https://dortania.github.io/OpenCore-Post-Install/
hackintools 

Other tools:
https://github.com/exelban/stats

