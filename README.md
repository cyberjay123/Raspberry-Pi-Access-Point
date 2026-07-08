# Raspberry Pi 5 Wireless Access Point Project

## Overview

This project demonstrates how to configure a Raspberry Pi 5 running Debian Linux as a wireless access point using hostapd, dnsmasq, and nftables. The goal was to create a secure Wi-Fi network while gaining hands-on experience with Linux administration, networking, and security concepts.

## Objectives

* Configure a Raspberry Pi 5 as a wireless access point
* Provide DHCP services to connected clients
* Enable DNS resolution
* Configure routing and network address translation (NAT)
* Strengthen Linux and networking skills
* Document deployment and troubleshooting procedures

## Technologies Used

### Hardware

* Raspberry Pi 5
* Ethernet connection
* Wi-Fi interface

### Software

* Debian Linux
* hostapd
* dnsmasq
* nftables
* OpenSSH

### Networking Concepts

* DHCP
* DNS
* NAT
* IP Forwarding
* TCP/IP
* Wireless Networking

## Skills Demonstrated

* Linux Administration
* Service Management
* Wireless Network Configuration
* DHCP and DNS Configuration
* Routing and NAT
* Network Troubleshooting
* Security Hardening

## Project Architecture

```text
Internet
    |
Home Router
    |
 Ethernet
    |
Raspberry Pi 5
(hostapd + dnsmasq)
    |
 Wi-Fi Access Point
    |
-------------------------
|      |      |         |
Phone Laptop Tablet Other
```

## Results

The Raspberry Pi successfully functioned as a wireless access point capable of:

* Broadcasting a custom SSID
* Providing DHCP services
* Resolving DNS requests
* Routing traffic between interfaces
* Supporting multiple wireless clients

## Future Improvements

* Captive portal integration using Nodogsplash
* VLAN implementation
* Client isolation policies
* Intrusion detection integration
* Enhanced monitoring and logging

## Setup Instructions

See `SETUP.md` for detailed installation and configuration steps.

## Resume Highlights

* Designed and deployed a Linux-based wireless access point using Raspberry Pi 5, hostapd, dnsmasq, and nftables.
* Configured DHCP, DNS, routing, and NAT services to support wireless client connectivity.
* Implemented wireless security controls and troubleshooting procedures in a Debian Linux environment.
