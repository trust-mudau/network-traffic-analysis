# HTTP vs HTTPS/TLS Analysis

## Objective

Compare unencrypted HTTP traffic with encrypted HTTPS/TLS traffic.

## HTTP Test

Example:

```text
curl http://example.com
```

### Wireshark Filter

```text
http
```

### Observation

Document what request/response details were visible.

## HTTPS Test

Visit an HTTPS website in your browser.

### Wireshark Filter

```text
tls
```

### Observation

Document what metadata is visible and what application content is not readable in plaintext.

## Comparison

| Feature | HTTP | HTTPS/TLS |
|---|---|---|
| Application content readable in normal capture | | |
| Encryption | | |
| Transport typically uses TCP | | |
| Security benefit | | |

## Security Relevance

Explain why encryption protects application data in transit while still leaving some network metadata observable.

## Evidence

Add screenshot filename(s) here.
