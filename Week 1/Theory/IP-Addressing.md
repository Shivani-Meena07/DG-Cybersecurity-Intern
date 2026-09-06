# IP Addressing

## Introduction

An IP address is a logical address assigned to a device on a network. It helps identify the device and allows data to be delivered to the correct destination.

Two commonly used versions are IPv4 and IPv6.

An IPv4 address consists of four numbers separated by periods.

Example:

```text
192.168.1.10
```

---

## Public and Private IP Addresses

### Private IP Address

A private IP address is used within a local network, such as a home, college, or office network.

Common private IPv4 ranges include:

* 10.0.0.0 to 10.255.255.255
* 172.16.0.0 to 172.31.255.255
* 192.168.0.0 to 192.168.255.255

Example:

```text
192.168.1.10
```

Private addresses are not directly routable over the public Internet.

---

## Public IP Address

A public IP address is used to identify a network or device on the public Internet.

Internet service providers assign public IP addresses to customer networks.

For example, a home router may have a public IP address on its Internet-facing interface while devices inside the home use private IP addresses.

---

# Basic Subnetting Concept

Subnetting is the process of dividing a larger IP network into smaller logical networks called subnets.

A subnet mask helps determine which portion of an IPv4 address represents the network and which portion represents the host.

For example:

```text
IP Address:    192.168.1.10
Subnet Mask:   255.255.255.0
```

The subnet mask can also be represented using CIDR notation:

```text
192.168.1.10/24
```

A `/24` network commonly represents:

```text
Network: 192.168.1.0
```

with host addresses available within that network.

For a typical `/24` IPv4 subnet:

* Network address: `192.168.1.0`
* Usable host range: `192.168.1.1` to `192.168.1.254`
* Broadcast address: `192.168.1.255`

This gives 254 usable host addresses.

---

## Why Subnetting Is Used

Subnetting can be used to:

* Organize networks
* Reduce unnecessary broadcast traffic
* Improve network management
* Separate different groups of devices
* Use IP address space efficiently

### Real-Life Example

A college network can be divided into separate subnets for:

* Students
* Faculty
* Administration
* Computer laboratories

This helps organize and manage the network more effectively.

---

## IP Addressing Summary

| Concept     | Description                                                    |
| ----------- | -------------------------------------------------------------- |
| IP Address  | Logical address used to identify a device/network              |
| Public IP   | Address used on the public Internet                            |
| Private IP  | Address used within a local network                            |
| Subnet Mask | Identifies network and host portions                           |
| Subnetting  | Dividing a network into smaller networks                       |
| CIDR        | Notation such as `/24` used to represent network prefix length |

## Conclusion

IP addressing is fundamental to networking because it allows devices and networks to identify each other and communicate. Understanding public and private addresses and the basic concept of subnetting provides a foundation for more advanced networking and cybersecurity concepts.
