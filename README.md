# powersave
Powersave for Dell Inspiron 15 Serie 5000 (i15-5558-B30)

Added modifications to Dell Inspiron 15 Serie 5000 (i15-5558-B30), and some extra goodies from the original script: https://github.com/quequotion/pantheon-bzr-qq/blob/master/EXTRAS/indicator-powersave/throttle


##Intall on paths:
```
/usr/lib/systemd/system-sleep/00-powersave"
/etc/udev/rules.d/99-powersave.rules"
/usr/bin/low-battery"
/usr/lib/systemd/system/low-battery.service"
/usr/lib/systemd/system/low-battery.timer"
/usr/bin/throttle"
```

##Archlinux

https://aur.archlinux.org/packages/powersave-git/
