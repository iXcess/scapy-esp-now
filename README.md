# ESP-Now Action Frame Manipulation

Python ESp-Now packet manipulation for communication between linux devices and ESP32 using scapy.

Most of the commercial drones uses the Open WiFi connection for easy user configuration. This basically means that the drone will act as an Access Point (AP) to which a controller normally a phone to connect. Open WiFi also means that most commercial and hobbyist drones uses the IEEE 802.11 protocol. 

## Characteristics of an AP

An AP will usually broadcast beacon frames. [Beacon frames] are transmitted periodically, they serve to announce the presence of a wireless LAN and to synchronise the members of the service set. It contains all the information about the network.

![Beacon frame from wireshark](https://3.bp.blogspot.com/-FKoOO4JgZPg/Tx2twnX4B9I/AAAAAAAAADU/pOI4zC1fTw4/s1600/wireshark-beacon-frame.png)

These beacon frames can be captured by Wireshark to be analysed to understand in-depth. However, we will use Scapy. [Scapy] is a Python interpreter that enables you to create, forge, or decode packets on the network, to capture packets and analyze them, to dissect the packets, etc. It also allows you to inject packets into the network. It supports a wide number of network protocols and it can handle and manipulate wireless communication packets.


### Prerequisites

Hardware required :
1. Wireless adapter which can go into monitor mode, a simple google about your laptop's wireless chipset can do. Or you can get an external [dongle which supports monitor mode]. I am using a wireless dongle with Atheros AR9271 chipset.

Software required :
1. Scapy

```
pip install scapy
```

## Contributing

Please contact me @ brandonting@hotmail.com if you feel like contributing or ask about any question.

## Versioning

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details

[Beacon frames]: https://en.wikipedia.org/wiki/Beacon_frame
[Scapy]: https://resources.infosecinstitute.com/what-is-scapy/#gref
[dongle which supports monitor mode]: https://www.wirelesshack.org/best-kali-linux-compatible-usb-adapter-dongles.html

