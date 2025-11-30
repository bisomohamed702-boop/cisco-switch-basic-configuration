# Cisco Switch Basic Configuration Lab

This project is a simple Packet Tracer lab demonstrating the fundamental configurations for a Cisco switch. These settings are essential for establishing a baseline for management and security on any new network device.

## Lab Topology

Here is the simple topology used in this lab, consisting of a single switch and a PC for management.

(We will add the topology image link here later)

---
## Configuration Steps

Below are the commands used to configure the switch, broken down by function.

### 1. Set Hostname
Switch(config)# hostname CCNA-SW

### 2. Secure Privileged EXEC Mode
Switch(config)# enable secret ccna

### 3. Secure Console Access
Switch(config-line)# password ccna
Switch(config-line)# login

### 4. Secure Remote Access (VTY Lines)
Switch(config-line)# password ccna
Switch(config-line)# login

### 5. Configure Management Interface (SVI)
Switch(config-if)# ip address 10.0.0.1 255.0.0.0
Switch(config-if)# no shutdown

### 6. Add a Warning Banner (MOTD)
Switch(config)# banner motd # Unauthorized access is strictly prohibited! #

### 7. Encrypt Plain-Text Passwords
Switch(config)# service password-encryption

### 8. Save the Configuration
CCNA-SW# copy running-config startup-config

---

## How to Use
1. Download the .pkt file.
2. Open it using Cisco Packet Tracer.
3. The password for all access is ccna.
4.
