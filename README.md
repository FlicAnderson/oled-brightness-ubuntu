# oled-brightness-ubuntu
Modified from the original https://wiki.archlinux.org/index.php/Dell_XPS_15_7590 to work
with Ubuntu and any locale

Further modified to work on my Ubuntu 18.04 Dell XPS 15 7590, with intel drivers fix. 
~~Previous version didn't work, as it operated on 'eDP-1' rather than 'eDP1' the display my system was looking for.~~
Turns out it DOES need to use `eDP-1`, instead of `eDP1`; I've amended this. 

Also need to do this: 

> Go to startup applications >
> Add:
> name: "brightness keys for intel display"
> command: /usr/local/bin/xbacklightmon
> comment: "magic script from github"
> Save.

> This adds it to the startup programs list.

...in order to get the script running at startup.
