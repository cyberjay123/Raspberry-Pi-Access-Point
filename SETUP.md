# Setup Instructions

## Prerequisites

### Hardware

* Raspberry Pi 5
* MicroSD card with Debian Linux installed
* Ethernet connection
* Power supply

### Software

* Debian Linux
* hostapd
* dnsmasq
* nftables

## Installation

Update the system:

```bash
sudo apt update
sudo apt upgrade -y
```

Install required packages:

```bash
sudo apt install hostapd dnsmasq nftables -y
```

Enable services:

```bash
sudo systemctl enable hostapd
sudo systemctl enable dnsmasq
sudo systemctl enable nftables
```

## Configuration

### hostapd

Configure hostapd to:

* Create a wireless SSID
* Enable WPA2 security
* Manage wireless client connections

### dnsmasq

Configure dnsmasq to:

* Assign IP addresses through DHCP
* Provide DNS services to clients

### Routing and NAT

Enable IP forwarding:

```bash
sudo sysctl -w net.ipv4.ip_forward=1
```

Configure NAT using nftables to allow wireless clients to access external networks through the Raspberry Pi.

## Verification

Verify that:

* The SSID is visible
* Clients receive an IP address
* DNS resolution works
* Internet connectivity is available
* Multiple devices can connect successfully

## Troubleshooting

### Check hostapd

```bash
sudo systemctl status hostapd
```

### Check dnsmasq

```bash
sudo systemctl status dnsmasq
```

### Check Routing

```bash
ip route
```

### Check Firewall Rules

```bash
sudo nft list ruleset
```

## Project Outcome

The Raspberry Pi successfully operated as a wireless access point, providing DHCP, DNS, routing, and internet connectivity for connected wireless devices.
 
