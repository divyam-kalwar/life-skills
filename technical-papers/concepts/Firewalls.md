# Firewalls

## Introduction

A firewall is a network security system that monitors and controls
incoming and outgoing network traffic based on predefined security
Rules: it serves as a barrier between a trusted network, such as a private
an office network, and a network that is not trusted, such as the Internet.
Firewalls help prevent unauthorized access while allowing legitimate
Communication methods can be provided in the form of hardware devices or software.
applications, or cloud-based services.

## How does a firewall work?

A firewall controls the flow of data between your computer or network and the internet. It acts like a barrier, letting safe data in and blocking harmful data. Firewalls use a set of rules to decide what traffic to allow or block. These rules can filter data by source, destination, port, or protocol. Some firewalls check only basic information, while others look closely at the content of each packet. By blocking unwanted traffic, a firewall helps keep your system safe from attacks and unauthorized access.

When data travels across a network, it is divided into smaller units
referred to as packets. A firewall examines the details of these packets and
It is compared with the security rules that have been configured. According to these rules,
The firewall determines if the traffic should be allowed or blocked.

For example, a firewall can allow web traffic using HTTPS while blocking
Links to services that are not allowed. This is helpful
administrators control which devices and services can communicate with
the network.

``` mermaid
flowchart LR
    A[Internet] --> B[Firewall]
    B -->|Allowed traffic| C[Private Network]
    B -->|Blocked traffic| D[Rejected traffic]
```

### Packet Filtering

A packet filtering firewall checks individual packets using information
such as source IP address, destination IP address, port number, and
A network protocol; it permits or blocks packets based on a set of
The method is simple and efficient, but it involves basic packet filtering.
It does not keep track of the full state of a network connection.

### Stateful Inspection

A stateful inspection firewall keeps track of active network
It keeps the information about connections in a state table and
It checks whether the incoming packets are part of a valid connection. This
allows it to make decisions using both firewall rules and the state of
the communication.

### Proxy Firewall

A proxy firewall works as an intermediary between a user's device and an
It does not permit a direct connection, instead receiving
It takes the requests and passes them on in accordance with the security policy. It can
inspect application-level traffic, but this additional processing may
affect network performance.

### Next-Generation Firewall

A next-generation firewall (NGFW) provides traditional firewall features
Together with extra security features, depending on the product,
these may include application awareness, intrusion prevention, deep
There is packet inspection and threat detection, and these features help
Organisations keep an eye on and regulate a greater variety of network activities.

## References

-   <https://www.cisco.com/site/us/en/learn/topics/security/what-is-a-firewall.html>
-   <https://csrc.nist.gov/pubs/sp/800/41/r1/final>
-   <https://www.youtube.com/watch?v=eO6QKDL3p1I&list=PLBbU9-SUUCwV7Dpk7GI8QDLu3w54TNAA6>
