# Useful Wireshark Display Filters

## Protocol Filters

```text
dns
icmp
tcp
udp
http
tls
arp
```

## IP Filters

Traffic to or from one IP:

```text
ip.addr == 192.168.1.10
```

Only packets sourced from an IP:

```text
ip.src == 192.168.1.10
```

Only packets sent to an IP:

```text
ip.dst == 192.168.1.10
```

## TCP Filters

TCP SYN packets:

```text
tcp.flags.syn == 1
```

Initial SYN packets without ACK:

```text
tcp.flags.syn == 1 && tcp.flags.ack == 0
```

TCP reset packets:

```text
tcp.flags.reset == 1
```

Traffic on a specific TCP port:

```text
tcp.port == 443
```

## DNS Filters

All DNS:

```text
dns
```

DNS queries:

```text
dns.flags.response == 0
```

DNS responses:

```text
dns.flags.response == 1
```

## Combining Filters

DNS or ICMP:

```text
dns || icmp
```

TCP traffic involving one IP:

```text
tcp && ip.addr == 192.168.1.10
```

## Notes

These are display filters. Display filters control what Wireshark shows after traffic has been captured; they do not retroactively change the packets stored in the capture.
