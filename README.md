# Extended-ACLs
Cisco Packet Tracer lab focused on configuring extended IPv4 ACLs to control network traffic based on source, destination, protocol, and port information.


# Extended Access Control Lists (ACLs)

## 📖 Overview

This lab focused on configuring and applying Extended Access Control Lists (ACLs) on Cisco routers to provide more granular control over network traffic.

Unlike Standard ACLs, which primarily filter traffic based on source IP addresses, Extended ACLs can make filtering decisions based on source and destination addresses, protocols, and port numbers.

## 🎯 Objectives

The lab was designed to:

* Understand the purpose of Extended ACLs.
* Configure extended IPv4 ACL rules.
* Control traffic based on source and destination IP addresses.
* Filter traffic based on protocols and port numbers.
* Apply ACLs to router interfaces.
* Understand ACL processing order.
* Verify ACL behavior.
* Test permitted and denied traffic.
* Troubleshoot ACL-related connectivity issues.

## 🧠 Concepts Practiced

* Extended ACLs
* IPv4 traffic filtering
* Source and destination IP filtering
* TCP and UDP filtering
* ICMP filtering
* Port-based filtering
* `permit` and `deny` statements
* ACL sequence and processing order
* Implicit deny
* Inbound and outbound ACL application
* Network access control

## 🛠️ Tools Used

* Cisco Packet Tracer
* Cisco IOS CLI

## ⚙️ Configuration

Extended ACL rules were configured on the router to define which types of traffic should be permitted or denied.

The rules could evaluate multiple packet characteristics, including:

* Source IP address
* Destination IP address
* Protocol
* TCP/UDP ports

The ACL was then applied to the appropriate router interface in the required direction.

## 🧪 Verification & Testing

The ACL configuration was verified using commands such as:

```text
show access-lists
show ip access-lists
show running-config
```

Connectivity and traffic behavior were tested using tools such as:

```text
ping <destination-ip>
```

Testing was performed from different hosts to verify that the ACL permitted legitimate traffic while blocking traffic that matched the configured restrictions.

## 🔍 Troubleshooting

Common ACL issues investigated during the lab included:

* Incorrect source or destination addresses.
* Incorrect protocol configuration.
* Incorrect port numbers.
* Applying the ACL to the wrong interface.
* Applying the ACL in the wrong direction.
* Incorrect ACL rule order.
* Unexpected traffic being blocked.
* Forgetting the implicit deny behavior.

Troubleshooting involved examining ACL entries, interface configurations, ACL counters, and performing targeted connectivity tests.

## 🔐 Security Concepts

Extended ACLs provide more precise traffic control than Standard ACLs because they can distinguish between different types of traffic.

For example, an administrator can allow a host to access a specific service while denying access to another service, rather than simply allowing or blocking all traffic from that host.

This makes Extended ACLs useful for implementing network segmentation and enforcing traffic-filtering policies.

## 📊 Standard vs Extended ACLs

| Feature                       | Standard ACL | Extended ACL  |
| ----------------------------- | ------------ | ------------- |
| Source IP                     | ✅            | ✅             |
| Destination IP                | ❌            | ✅             |
| Protocol                      | ❌            | ✅             |
| Port number                   | ❌            | ✅             |
| Traffic filtering granularity | Basic        | More specific |

## ✅ Outcome

Successfully configured and applied Extended IPv4 ACLs to control network traffic using source and destination addresses, protocols, and port information. ACL behavior was verified through configuration checks and connectivity testing.

## 📚 Skills Demonstrated

* Cisco IOS CLI
* Extended IPv4 ACL configuration
* Traffic filtering
* Source and destination filtering
* Protocol and port-based filtering
* Interface ACL application
* ACL verification
* Network security fundamentals
* Connectivity testing
* Network troubleshooting
