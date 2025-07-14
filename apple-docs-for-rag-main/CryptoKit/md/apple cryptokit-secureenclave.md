

- Apple CryptoKit
-  SecureEnclave 

Enumeration

# SecureEnclave

A representation of a device’s hardware-based key manager.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
enum SecureEnclave
```

## Topics

### Checking availability

static var isAvailable: Bool

A Boolean value that indicates if the device supports Secure Enclave access.

### Using the secure enclave

enum P256

An elliptic curve that enables NIST P-256 signatures and key agreement within the Secure Enclave.

## Relationships

### Conforms To

- Sendable

## See Also

### Public key cryptography

enum Curve25519

An elliptic curve that enables X25519 key agreement and Ed25519 signatures.

enum P521

An elliptic curve that enables NIST P-521 signatures and key agreement.

enum P384

An elliptic curve that enables NIST P-384 signatures and key agreement.

enum P256

An elliptic curve that enables NIST P-256 signatures and key agreement.

struct SharedSecret

A key agreement result from which you can derive a symmetric cryptographic key.

enum HPKE

A container for hybrid public key encryption (HPKE) operations.

