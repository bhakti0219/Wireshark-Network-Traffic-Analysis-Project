# Wireshark Security Analysis

## Objective

The objective of this analysis was to examine captured network traffic using Wireshark and identify potentially unusual communication patterns.

## Traffic Analyzed

The capture was analyzed for:

* TCP
* UDP
* DNS
* ICMP
* HTTP
* TLS
* IP addresses
* Network ports

## Observations

TCP traffic was analyzed to understand connection establishment and communication between hosts.

DNS traffic was examined to identify domain-name queries and responses.

ICMP traffic was observed during the Windows ping test.

TLS traffic was analyzed to understand encrypted network communication.

## Security Analysis

The capture was reviewed for repeated connection attempts, unusual ports, unexpected destinations, and unusual DNS activity.

Any unusual traffic should be investigated further using additional network logs, endpoint information, and security tools before determining whether it is malicious.

## Conclusion

Wireshark provided visibility into network-level communication and demonstrated how packet capture and protocol analysis can support basic network monitoring and SOC investigations.
