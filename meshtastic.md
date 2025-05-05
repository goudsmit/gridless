layout: page
title: "gridless - meshtastic radio-based mesh messaging"
permalink: /meshtastic

# meshtastic radio-based mesh messaging

In case mobile and fixed internet drop away, there is no way to reach relatives or friends to check in on them.

Meshtastic is an open source project, with open source hardware, to setup a mesh network of small radio-based devices,
that require little power, and can send text-messages between them. The system supported end to end encryption, private
messages, group chats via 'channels', and can easily stay charged with a small solar panel.

## items i've used

- Heltec v3, revision 3.2 (comes with small antenna)
- 103450 3.3V LiPo battery with micro JST 1.25mm 2-pin connector
- self-printed H1 extra wide case
- optional larger antenna for more range
- optional solar panel with USB-C 5V output

## steps for operation

- attach antenna (apparently sending messages without antenna can damage the unit)
- attach to computer via USB-C
- go to the meshtastic flash page and flash the firmware onto it
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

