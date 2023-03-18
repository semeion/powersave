# powersave
Powersave for Dell Inspiron 15 Serie 5000 (i15-5558-B30)

Added modifications to Dell Inspiron 15 Serie 5000 (i15-5558-B30), and some extra goodies from the original script: https://github.com/quequotion/pantheon-qq

The script is 10 times faster than the original and meet shellcheck specifications.


## Intall on paths:
```
/etc/throttle/powersave
  config file used to select powersave state

/etc/throttle/performance
  config file used to select performance state

/usr/lib/systemd/system-sleep/00-powersave
  systemd hook to run the script from suspend, hibernate, hybrid-sleep or resume events
  https://wiki.archlinux.org/title/Power_management#Hooks_in_/usr/lib/systemd/system-sleep

/etc/udev/rules.d/99-powersave.rules
  udev rules to run the script from power supply events

/usr/bin/low-battery
  script used to hibernate on low battery

/usr/lib/systemd/system/low-battery.service
  low_battery systemd unit to be called by timer

/usr/lib/systemd/system/low-battery.timer
  runs low-battery every 5 minutes

/usr/bin/throttle
  main script
```

## Archlinux

https://aur.archlinux.org/packages/powersave-git/
