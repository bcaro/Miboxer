# Miboxer
Miboxer : a bridge to control Milight bulbs

The new brand Miboxer replaces MiLight a brand from Futlight. With bridges iBox1 and iBox2 a simple protocol was used to dialog between the app and the bridge.
see : 

https://github.com/yasharrashedi/LimitlessLED

The Miboxer is completely different and uses the Tuya protocol. The tuya local protocol is explained here :

https://github.com/Marcus-L/m4rcus.TuyaCore

https://github.com/codetheweb/homebridge-tuya

It is then possible to dialog with Tuya devices in LAN mode i.e. without internet. The difficulty is to find the id and key needed for the dialog between device and app. It is easily to retreive them using packet capture during the dialog between Smart Life app and the device.

For the Miboxer a new app MiBoxer is used to dialog with bulbs but the VPN used by packet capture is detected by the app and it is not possible to retrive Id and key.

It is possible to SmartFile to pair with the Miboxer and then to obtain the key. But the only command that is available is :

{dps:{"20":false}} and true

but it is impossible to find the orther commands for brightness, color, kelvin with SmartLive app.






