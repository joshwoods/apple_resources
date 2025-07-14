

- Apple CryptoKit
- SecureEnclave
- SecureEnclave.P256
-  SecureEnclave.P256.KeyAgreement 

Enumeration

# SecureEnclave.P256.KeyAgreement

A mechanism used to create a shared secret between two users by performing NIST P-256 elliptic curve Diffie Hellman (ECDH) key exchange within the Secure Enclave.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
enum KeyAgreement
```

## Topics

### Using keys

struct PrivateKey

A P-256 private key used for key agreement.

## Relationships

### Conforms To

- Sendable

## See Also

### Performing operations

enum Signing

A mechanism used to create or verify a cryptographic signature using the NIST P-256 elliptic curve digital signature algorithm (ECDSA) within the Secure Enclave.

