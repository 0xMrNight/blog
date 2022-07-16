---
title: "MAC Addresses"
description: "Media Access Control addresses and its types"
date: "2022-07-16 11:30:00 +05:30"

author: "Siddharth Arumugam"
authorTwitter: "0xMrNight"

tags: ["computer-networking", "mac-address"]
keywords: ["mac-address", "network", "network-interface"]

showFullContent: false
---

## What is a MAC Address?

A media access control (MAC) address is a unique identification number assigned to every network interface controller (NIC). 

MAC addresses are assigned by the device manufacturer and are burned-in to the NIC.

MAC Addresses are also called 

- _Burned-in address_: as the address is burned into the Read-only Memory (ROM) of the NIC,
- _Physical address_: The MAC address is the unique hardware address of every NIC,
- _Hardware address_
- _Ethernet hardware address_

## Structure of MAC Address

A MAC address is a 48-bit address. It has 6 groups of 2 hexadecimal digits.

![MAC Address format](https://cdn.jsdelivr.net/gh/0xMrNight/blog-images@master/2022/07/mac-addresses/mac-address.webp)

The 6 octets are separated by colons (:), hyphens (-), or left without a separator. 

#### Organizationally Unique Identifier 

The first 3 octets of a MAC address represent the manufacturer of the NIC.

The OUI are assigned by the IEEE Registration Authority.

For example, 

| OUI      | Organization       |
| ----     | ------------       |
| AC:ED:5C | Intel Corporate    |
| CC:46:D6 | Cisco Systems, Inc |
| F8:8F:CA | Google, Inc.       |
| C4:2A:D0 | Apple, Inc.        |

> Manufacturers usually have multiple OUIs. The full list of OUIs is [here](https://standards-oui.ieee.org/oui/oui.txt).

Some virtualisation softwares have their own OUIs, such as VMware (`00:50:56`), QEMU (`52:54:00`), etc.

#### Network Interface Controller

The NIC is the hardware component that connects a device to the network, such an adapter or card.

The last 3 octets of the MAC address identify the NIC.
