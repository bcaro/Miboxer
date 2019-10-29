# Miboxer
Miboxer : a bridge to control Milight bulbs

The new brand Miboxer replaces MiLight a brand from Futlight. With bridges iBox1 and iBox2 a simple protocol was used to dialog between the app and the bridge. See : 

https://github.com/yasharrashedi/LimitlessLED

The Miboxer is completely different and uses the Tuya protocol. The tuya local protocol is explained here :

https://github.com/Marcus-L/m4rcus.TuyaCore

https://github.com/codetheweb/homebridge-tuya

It is then possible to dialog with Tuya devices in LAN mode i.e. without internet. The difficulty is to find the id and key needed for the dialog between device and app. It is easy to retreive them using packet capture during the dialog between Smart Life app and the device.

For the Miboxer a new app MiBoxer is used to dialog with bulbs but the VPN used by packet capture is detected by the app and it is not possible to retrive Id and key.

Fortunetly, It is possible to pair the MiBoxer bridge with SmartFile and then to obtain the key. But the only commands that are available in LAN mode are:

{dps:{"20":false}} {dps:{"20":true}}

The other commands for brightness, color, kelvin givern by SmartLive are not available dor the MiBoxer.






