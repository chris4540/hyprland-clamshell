# hyprland-clamshell

A user systemd service with scripts for hyprland notebook user

## Scenario

Hyprland reload or updating the hyprland.conf shall make the clammed desktop reopen.
Thus, I created the a clamshell service with a script to monitor the notebook lid status

According to the monitor name convention, the laptop monitor is always starting with 'e'.
Thus, we can have a script to keep:
    1. when the lid is off, then the embedding monitor is off, and 
    2. when the lid is one and the only monitor is off, then enable it.

## Known issue

1. conntected with external monitor => sleep with swaylock => unplug => wake up => red screen.

## Reference
1. https://bobbys.zone/guides/hyprland-clamshell
