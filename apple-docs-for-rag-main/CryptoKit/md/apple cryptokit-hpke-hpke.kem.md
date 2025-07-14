

- Apple CryptoKit
- HPKE
-  HPKE.KEM 

Enumeration

# HPKE.KEM

The key encapsulation mechanisms to use in HPKE.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
enum KEM
```

## Topics

### Enumeration Cases

case Curve25519_HKDF_SHA256

A key encapsulation mechanism using X25519 elliptic curve key agreement and SHA-2 hashing with a 256-bit digest.

case P256_HKDF_SHA256

A key encapsulation mechanism using NIST P-256 elliptic curve key agreement and SHA-2 hashing with a 256-bit digest.

case P384_HKDF_SHA384

A key encapsulation mechanism using NIST P-384 elliptic curve key agreement and SHA-2 hashing with a 384-bit digest.

case P521_HKDF_SHA512

A key encapsulation mechanism using NIST P-521 elliptic curve key agreement and SHA-2 hashing with a 512-bit digest.

## Relationships

### Conforms To

- CaseIterable
- Equatable
- Hashable
- Sendable

## See Also

### Choosing cryptographic algorithms

struct Ciphersuite

Cipher suites to use in hybrid public key encryption.

enum AEAD

The authenticated encryption with associated data (AEAD) algorithms to use in HPKE.

enum KDF

The key derivation functions to use in HPKE.

enum DHKEM

A container for Diffie-Hellman key encapsulation mechanisms (KEMs).

