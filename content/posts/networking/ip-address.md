---
title: "IP Addresses"
description: "A basic overview of the Internet Protocol, IP addresses and its types."
date: "2022-06-30 20:00:00 +05:30"

author: "Siddharth Arumugam"
authorTwitter: "0xMrNight"

tags: ["computer-networking", "ip"]
keywords: ["ip", "ip-address", "network"]

showFullContent: false
---

## Internet Protocol

The Internet Protocol (IP) is the protocol by which data is sent across the Internet.

## What is an IP address?

An IP address is a unique string of numbers assigned to every device connected to the Internet.

## Types of IP addresses

#### Dynamic IP

Dynamic IP addresses are temporary addresses that change from time to time.

They are assigned to devices on a network by the Dynamic Host Configuration Protocol (DHCP).

#### Static IP

Static IP addresses are permanent addresses that do not change until the device is decommissioned.

#### Public IP

Public (or) external IP addresses can be accessed directly over the Internet and are used for external communications.

Public IP addresses are assigned to a router or network by the Internet Service Provider (ISP).

#### Private IP

Private (or) internal (or) local IP addresses are assigned to all devices connected to a network. They are the same for any network.

**Ranges**: 

* Class A: `10.0.0.0` to `10.255.255.255`
* Class B: `172.16.0.0` to `172.31.255.255`
* Class C: `192.168.0.0` to `192.168.255.255`

_Note: These are [IPv4](#ipv4) addresses (more on that later)_

#### Shared IP

A shared IP address is used by multiple domains or websites.

#### Dedicated IP

A dedicated IP address is an address allotted exclusively to one website.

#### Loopback IP

Data sent to a loopback address are looped and sent back to the device.

They are managed entirely within the operating system (the data never reaches the network).

**Range**: `127.0.0.0` to `127.255.255.255` (IPv4) 

The most common loopback address is _localhost_ (IPv4: `127.0.0.1`, IPv6: `::1`).

## Versions of IP

Currently, there are two version of IP publicly used - IPv4 and IPv6.

#### IPv4

Internet Protocol version 4 (IPv4) is the first public version of the IP.

IPv4 is a 32-bit address. It has 4 octets.

![IPv4 format](https://cdn.jsdelivr.net/gh/0xMrNight/blog-images@master/2022/06/ip-addresses/ipv4-format.webp)

> In November 2019, we ran out of _unallocated_ IPv4 addresses. However, IPv4 addresses continue to be in use and will most likely coexist with IPv6 for many years.

#### IPv6

Internet Protocol version 6 (IPv6) is the second public version of the IP, intended to become a successor to IPv4.

IPv6 is a 128-bit address. It has 16 octets. Each octet ranges from 0000 to FFFF (hexadecimal values).
