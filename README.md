# ESP-Now Action Frame Manipulation

Python ESP-Now packet manipulation for communication between linux devices and ESP32 using scapy. [Scapy] is a Python interpreter that enables you to create, forge, or decode packets on the network, to capture packets and analyze them, to dissect the packets, etc. It also allows you to inject packets into the network. It supports a wide number of network protocols and it can handle and manipulate wireless communication packets.

### Prerequisites

Hardware required :
1. Wireless adapter which can go into monitor mode, a simple google about your laptop's wireless chipset can do. Or you can get an external [dongle which supports monitor mode]. I am using a wireless dongle with Atheros AR9271 chipset.

Software required :
1. Scapy

```
pip install scapy
```

Make sure that your WiFi card has entered monitor mode. It is possible to do this with some googling, I am going to show how to do that in Linux:

```
ifconfig <interface> down

iwconfig <interface> mode monitor

ifconfig <interface> up
```

or if you have installed aircrack suite:

```
airmon-ng start <interface>
```

### Launching Scapy

In Linux, make sure you are root before running scapy.
![Scapy Interface](scapy.jpg)


## Contributing

Please contact me @ brandonting@hotmail.com if you feel like contributing or ask about any question.

## Versioning

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details

[Beacon frames]: https://en.wikipedia.org/wiki/Beacon_frame
[Scapy]: https://resources.infosecinstitute.com/what-is-scapy/#gref
[dongle which supports monitor mode]: https://www.wirelesshack.org/best-kali-linux-compatible-usb-adapter-dongles.html

