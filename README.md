available-ssid
======================
A script to print all the available networks on a wifi interface. It displays the BSSID, SSID, Channels, Frequency and sort them by RSSI.
Should work with most Debian-based distributions

Installation
------------
To download the latest version run:
```
git clone https://github.com/Resethel/available-ssid.git
```
You can then move the executable to your usual execution path
```
$ mv ./available-ssid /usr/local/bin
$ chmod 755 /usr/local/bin/available-ssid
```

Usage:
------
To display the available networks, run the command
```
available ssid <device_name> [-h|-p|-q]
```
Where:
- device_name is the name of you wifi device (you can find it with the ip command)
- You can display the available options with the option -h or --help

Output:
-------
Example of quiet and pretty output :
```
BSSID              RSSI     CH    Freq    SSID
                   (dBm)          (Mhz)
===============================================================
xx:xx:xx:xx:xx:xx  -12.00    4    2427    My-own-wifi
xx:xx:xx:xx:xx:xx  -44.00   11    2462    Neighbor-1-Wifi
xx:xx:xx:xx:xx:xx  -44.00   11    2462    Neighbor-2-Wifi
xx:xx:xx:xx:xx:xx  -73.00   44    5220    random-switch-foo
xx:xx:xx:xx:xx:xx  -89.00   52    5260    random-switch-bar
xx:xx:xx:xx:xx:xx  -89.00   52    5260    random-switch-baz
===============================================================

```
