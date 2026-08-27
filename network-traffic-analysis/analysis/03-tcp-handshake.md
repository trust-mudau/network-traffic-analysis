# TCP Three-Way Handshake Analysis

## Objective

Identify and explain the TCP three-way handshake.

## Wireshark Filter

```text
tcp.flags.syn == 1
```

For the initial SYN only:

```text
tcp.flags.syn == 1 && tcp.flags.ack == 0
```

## Packets Identified

| Stage | Source | Destination | Flags |
|---|---|---|---|
| 1 | | | SYN |
| 2 | | | SYN, ACK |
| 3 | | | ACK |

## Explanation

### 1. SYN
Explain what the client is requesting.

### 2. SYN-ACK
Explain what the server is acknowledging.

### 3. ACK
Explain why the final ACK establishes the connection.

## Security Relevance

Consider:
- Repeated SYN packets
- Incomplete handshakes
- Connection attempts to unusual ports
- Why handshake behavior can help identify scanning or connection problems

## Evidence

Add screenshot filename(s) here.
