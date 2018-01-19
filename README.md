rogdrv
------

rogdrv is a simple ASUS ROG Pugio userspace mouse driver for Linux.
The mouse device consists of 2 input devices: mouse and keyboard.
The keyboard part is unsupported on Linux, but it's recognised as HID device.
So this driver maps HID events to the generic keyboard events.

There is a chance that a driver can be compatible with other mouse devices
from ASUS ROG (Republic of Gamers) series.

The protocol was reverse-engineered, so everything is experimental. Use at your own risk.

Requirements
============

* python >= 3.0
* python-hidapi
* python-evdev

Features
========

* Virtual uinput device
* Button bindings
* LED colors

Using
=====

You need r/w permissions for /dev/hidrawX file for your mouse.

```
sudo ./rogdrv
```