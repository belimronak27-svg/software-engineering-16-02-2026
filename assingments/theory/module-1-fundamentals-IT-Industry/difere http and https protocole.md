# HTTP vs HTTPS Protocols

## Overview
- **HTTP** (HyperText Transfer Protocol): Unencrypted, standard web protocol
- **HTTPS** (HyperText Secure Transfer Protocol): Encrypted version of HTTP with SSL/TLS

## Key Differences

| Feature | HTTP | HTTPS |
|---------|------|-------|
| **Encryption** | None | SSL/TLS encrypted |
| **Port** | 80 | 443 |
| **Security** | Low | High |
| **Data Exposure** | Visible to intermediaries | Encrypted end-to-end |
| **Certificate** | Not required | Required (CA-signed) |
| **Performance** | Faster | Slightly slower (encryption overhead) |

## Security Implications

### HTTP Vulnerabilities
- Data transmitted in plaintext
- Susceptible to man-in-the-middle attacks
- No server authentication
- Vulnerable to eavesdropping

### HTTPS Benefits
- Encrypted communication channel
- Server authentication via certificates
- Data integrity verification
- Protection against tampering
- Required for sensitive data (logins, payments)

## Modern Best Practices
- Always use HTTPS for production applications
- Use HTTP only for non-sensitive content or redirects
- Implement HSTS (HTTP Strict Transport Security)
- Keep SSL/TLS certificates updated