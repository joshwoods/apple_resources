

- Apple CryptoKit
- P384
-  P384.Signing 

Enumeration

# P384.Signing

A mechanism used to create or verify a cryptographic signature using the NIST P-384 elliptic curve digital signature algorithm (ECDSA).

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
enum Signing
```

## Topics

### Using keys

struct PrivateKey

A P-384 private key used to create cryptographic signatures.

struct PublicKey

A P-384 public key used to verify cryptographic signatures.

### Structures

struct ECDSASignature

A P-384 elliptic curve digital signature algorithm (ECDSA) signature.

## Relationships

### Conforms To

- Sendable

## See Also

### Performing operations

enum KeyAgreement

A mechanism used to create a shared secret between two users by performing NIST P-384 elliptic curve Diffie Hellman (ECDH) key exchange.

