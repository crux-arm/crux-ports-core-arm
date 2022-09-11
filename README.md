# crux-ports-core-arm

CRUX-ARM ports overlay for CRUX core collection

To use these ports, download the `core-arm.httpup` file to `/etc/ports`:
```
$ sudo wget -P /etc/ports https://raw.githubusercontent.com/crux-arm/crux-ports-core-arm/main/core-arm.httpup
$ sudo ports -u core-arm
```

You may want to list it first in `/etc/prt-get.conf` to take advantage of ports overlay:
```
###
### prt-get conf
###

# note: the order matters: the package found first is used
prtdir /usr/ports/core-arm
prtdir /usr/ports/opt-arm
prtdir /usr/ports/xorg-arm
prtdir /usr/ports/core
prtdir /usr/ports/opt
prtdir /usr/ports/xorg
```
 
