# IP-Address-and# IP Address and MAC Address

## Introduction

In computer networking, every device needs an identity so that it can communicate with other devices. Two important types of addresses are:

1. **IP Address**
2. **MAC Address**

Both are used for communication, but they work at different layers and have different purposes.

---

# 1. IP Address

## Definition

An **IP (Internet Protocol) Address** is a logical address assigned to a device on a network.

It is used to identify a device and help deliver data from one network to another.

### Example

IPv4 address:

`192.168.1.10`

IPv6 address:

`2001:db8::1`

## Types of IP Address

### IPv4

IPv4 uses **32 bits** and is normally written in four decimal parts.

Example:

`192.168.1.10`

### IPv6

IPv6 uses **128 bits** and is written using hexadecimal numbers.

Example:

`2001:db8:85a3::8a2e:370:7334`

## Public IP

A **Public IP** is an address used to identify a network or device on the Internet.

## Private IP

A **Private IP** is used inside a local network, such as a home, school, or office network.

Common private IPv4 ranges include:

* `10.0.0.0 – 10.255.255.255`
* `172.16.0.0 – 172.31.255.255`
* `192.168.0.0 – 192.168.255.255`

---

# 2. MAC Address

## Definition

A **MAC (Media Access Control) Address** is a hardware/network-interface address used for communication on a local network.

It is associated with a network interface, such as an Ethernet or Wi-Fi adapter.

### Example

`00:1A:2B:3C:4D:5E`

A MAC address is commonly represented as **48 bits** in hexadecimal notation.

## Purpose of MAC Address

A MAC address helps devices identify each other on a **local network**.

For example:

**Laptop → Switch/Access Point → Other Device**

The local network uses MAC addresses to deliver Ethernet/Wi-Fi frames to the appropriate network interface.

---

# Difference Between IP Address and MAC Address

| Feature        | IP Address                             | MAC Address                                           |
| -------------- | -------------------------------------- | ----------------------------------------------------- |
| Full Form      | Internet Protocol Address              | Media Access Control Address                          |
| Type           | Logical address                        | Hardware/network-interface address                    |
| Main Use       | Identifies and routes devices/networks | Identifies a network interface on the local network   |
| Example        | `192.168.1.10`                         | `00:1A:2B:3C:4D:5E`                                   |
| Common Version | IPv4 / IPv6                            | Usually 48-bit MAC                                    |
| Can change?    | Yes                                    | Can be changed/spoofed in software in some situations |
| Used Mainly At | Network Layer                          | Data Link Layer                                       |

---

# IP Address and MAC Address Together

When a device communicates on a local network, both addresses can be involved.

For example:

**IP Address:** `192.168.1.10`
**MAC Address:** `00:1A:2B:3C:4D:5E`

The IP address helps with logical network communication, while the MAC address is used for local-link delivery.

### Simple Example

Suppose a laptop wants to communicate with another device on the same local network.

1. The laptop knows the destination **IP address**.
2. It can use **ARP** in IPv4 to discover the destination MAC address.
3. The data is sent across the local network using the destination MAC address.
4. The IP information is used for the logical communication between devices.

---

# Cyber Security Importance

IP and MAC addresses are important in Cyber Security because they help security professionals identify and monitor devices on a network.

They can be useful for:

* Network monitoring
* Device identification
* Access control
* Troubleshooting
* Detecting unusual network activity
* Investigating network incidents

Security professionals should remember that an IP address or MAC address alone does **not** prove who a person is. Devices and addresses can change, and MAC addresses can sometimes be spoofed.

---

# Useful Commands

## Windows

To view IP and MAC information:

```text
ipconfig /all
```

To view the ARP table:

```text
arp -a
```

## Linux / Kali Linux

To view network interface and IP information:

```bash
ip addr
```

To view MAC addresses:

```bash
ip link
```

To view the ARP/neighbour table:

```bash
ip neigh
```

---

# Conclusion

An **IP address** is a logical address used for communication and routing, while a **MAC address** identifies a network interface on the local network.

### Easy Way to Remember

**IP = Logical Address**

**MAC = Network Interface Address**

Both are important for understanding how networks communicate and how Cyber Security professionals monitor and protect networks.
-MAC-Address
