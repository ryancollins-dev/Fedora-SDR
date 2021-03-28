# SDR On Fedora

## Working with GQRX

[Dongle](https://www.nooelec.com/store/sdr/sdr-receivers/nesdr-smart-sdr.html)

## Steps

> sudo dnf group install 'Electronic Lab'

> sudo dnf install rtl-sdr gr-osmosdr

Blacklist default driver

> cd /etc/modprobe.d

Create a file

> vi blacklist-dvb.conf

cat blacklist-dvb.conf

>blacklist dvb_usb_rtl28xxu


Next plug in dongle, attach antenna

> rtl_test

then ctrl-c once you see output

## Software

Grab binary from here -> https://github.com/csete/gqrx

> ./gqrx

If all goes well, you select, your dongle from sources when it opens

![GQRX](/img/Screenshot.png)
