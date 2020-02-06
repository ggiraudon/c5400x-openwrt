# c5400x-openwrt

This is an effort to bring OpenWRT to the Archer C5400X
At this time, there is no functional code or image here. Just preliminary data and guess work.


The offical web page for the router is :
https://www.tp-link.com/ca/home-networking/wifi-router/archer-c5400x/

An archive containing the GPL code used in making TP-Link's firmware is located at :
https://static.tp-link.com/resources/gpl/AC5400Xv1_GPL.tar.gz

Hardware Specifications :
CPU : Broadcom 4908
Radio : Broadcom 4366

Some preliminary thoughts/notes :

The router has a 4 pin connector on the board that has a 3.3v VCC and GND pin as well as 2 unknown ones.
It is probably a UART but I am unable to get anything from it yet. Some jumpers or bridges might have been purposefuly been left unconnected.

The GPL archive seems to be vastly incomplete.

The firmware is actually OpenWRT modified and reskinned by TP-Link
The fs even contains the /etc/openwrt_version and openwrt_release files
This is the openwrt_release file content :

DISTRIB_ID="OpenWrt"
DISTRIB_RELEASE="Attitude Adjustment"
DISTRIB_REVISION="unknown"
DISTRIB_CODENAME="attitude_adjustment"
DISTRIB_TARGET="model_brcm_bcm490x/generic"
DISTRIB_DESCRIPTION="OpenWrt Attitude Adjustment 12.09-rc1"


Non of the OpenWRT code is included in the GPL archive published by TP-Link.
Nor does it make any reference to it.
