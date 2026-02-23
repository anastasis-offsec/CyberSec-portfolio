# Wireless Security Assessment Lab
Author: Anastasis Tsiropoulos  

---

## 1. Objective
Demonstrate wireless security assessment techniques in a controlled lab
environment using Kali Linux and an Atheros USB adapter.

---


⚠️ All tests were performed on my own lab network created for educational purposes.

---
Wireless Penetration Testing Lab Report
1. Objective

The objective of this lab was to perform a security assessment of a wireless network in order to evaluate its resilience against common Wi-Fi attacks and identify potential weaknesses in WPA2 authentication.

All testing was conducted on a privately owned network for educational and authorized purposes only.

2. Testing Environment

Operating System: Kali Linux

Wireless Adapter: Atheros chipset (monitor mode supported)

Target Network: WPA2-PSK secured wireless network

Virtualization Platform: VMware / VirtualBox (adjust based on what you used)

Tools Used

Aircrack-ng suite

Airodump-ng

Aireplay-ng

Airmon-ng

3. Methodology
3.1 Enabling Monitor Mode

The wireless adapter was switched to monitor mode in order to capture raw 802.11 packets.

This allowed passive monitoring of nearby wireless networks.

3.2 Network Discovery

A wireless scan was performed to identify available access points.

The following parameters were enumerated:

SSID

BSSID

Channel

Encryption type

Signal strength

Connected clients

3.3 Handshake Capture

The target access point was isolated using its BSSID and channel.

A WPA2 handshake was captured during client authentication.

To accelerate the process, a controlled deauthentication attack was performed against a connected client to force reauthentication and capture the handshake.

3.4 Password Analysis

An offline dictionary attack was conducted against the captured handshake using a wordlist.

The purpose was to evaluate password strength and resistance to brute-force/dictionary attacks.

4. Findings

The network was secured using WPA2-PSK encryption.

A valid 4-way handshake was successfully captured.

Password strength evaluation:

Weak / Moderate / Strong (adjust based on your result)

No additional wireless-layer vulnerabilities were identified during this assessment.

5. Security Recommendations

Upgrade to WPA3 where available

Use a password longer than 14 characters

Avoid dictionary-based or predictable passwords

Disable WPS

Regularly update router firmware

Monitor unknown client connections



---

