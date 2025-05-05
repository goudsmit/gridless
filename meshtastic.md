# meshtastic radio-based mesh text messaging

In case mobile and fixed internet drop away, there is no way to reach relatives or friends to check in on them.

[Meshtastic](https://meshtastic.org/) is an open source project, with open source hardware, to setup a mesh network
of small radio-based devices, that require little power, and can send text-messages between them. The system
supported end to end encryption, private messages, group chats via 'channels', and can easily stay charged with
a small solar panel.

## items i've used

- [Heltec v3, revision 3.2](https://www.tinytronics.nl/en/development-boards/microcontroller-boards/with-lora/heltec-wifi-lora-32-esp32-s3-sx1262-with-0.96-inch-oled-display) (comes with small antenna)
- [103450 3.3V LiPo battery with micro JST 1.25mm 2-pin connector](https://www.amazon.de/dp/B08TQSC5G9)
- self-printed [H1 extra wide case](https://makerworld.com/en/models/591051-h1-big-case-for-heltec-v3-running-meshtastic)
- [optional larger adjustable antenna for more range](https://www.amazon.de/dp/B0DY1LDBQ8)
- [optional solar panel with USB-C 5V output](https://www.amazon.de/dp/B0CLDVS4D7)

## steps for operation

- attach antenna (apparently sending messages without antenna can damage the unit)
- attach to computer via USB-C
- go to the [meshtastic flash page](https://flasher.meshtastic.org/) and flash the firmware onto it
- install and open the meshtastic app on your phone
- go to the bluetooth tab, and connect & pair to your node
- select EU 868 as operating frequency band
- the node can now already connect to the mesh and send and receive messages on the public channel

## steps for customizing

- change the name and shortname
- I just changed 'meshtastic' to 'Goldtastic' for my nodes, keeping the suffix
- I change the shortname to colors/materials, first letter matching the use, and printed mathing enclosures
- add channels you want to receive messages for; I made one for my family, and one for my group of friends

## administration

- if you want to remote-admin nodes, configure their admin keys with the public key of the node you will use locally
- if you want to place those nodes at people's places who should be able to use them, check 'managed mode'
- if you are making a node just to strengthen the mesh, set role to client-mute

