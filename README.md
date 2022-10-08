# Linux Settings

## Natural Scrolling on i3wm
```
sudo emacs /usr/share/X11/xorg.conf.d/40-libinput.conf
```

Then add like th following to pointer and touchpad and restart i3:

```
Section "InputClass"
        Identifier "libinput touchpad catchall"
        MatchIsTouchpad "on"
        MatchDevicePath "/dev/input/event*"
        Driver "libinput"
	Option "NaturalScrolling" "True"
EndSection
```


## Add Webstorm to your PATH Variables

```
sudo ln -s ~/WebStorm-222.4167.31/bin/webstorm.sh /usr/local/bin/webstorm
```

To remove symlink:

```
rm /usr/local/bin/webstorm
```

## Gnome Settings
```
gnome-control-center
```
