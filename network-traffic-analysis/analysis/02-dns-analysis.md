# DNS Traffic Analysis

## Objective

Observe how a hostname is translated into an IP address using DNS.

## Test Performed

Command or action used:

```text
nslookup example.com
```

## Wireshark Filter

```text
dns
```

## Observation

### DNS Query

- Source IP:
- Destination IP:
- Query name:
- Query type:
- Transaction ID:

### DNS Response

- Source IP:
- Destination IP:
- Resolved IP address(es):
- Response code:

## What Happened?

Write a short explanation of how your computer asked a DNS resolver for the IP address associated with the hostname and how the resolver responded.

## Security Relevance

Consider:
- Why DNS logs are useful to defenders
- How unusual domains may indicate suspicious activity
- Why DNS does not automatically mean malicious activity

## Evidence

Add screenshot filename(s) here.
