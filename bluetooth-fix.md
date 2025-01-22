# Problem

Bluetooth seemingly stopped working alltogether on Linux Mint 21.3. Attempts at launching `blueman` failed as nothing would launch or show in processes.

# Solution
> remove the bluez protocol stack and the blueman manager and reinstall both which seems to rebuild some default Bluetooth audio config files automatically that were missing

```
sudo apt purge bluez
sudo apt install bluez
sudo apt install blueman
reboot
```

# Reference
https://forums.linuxmint.com/viewtopic.php?t=425923
