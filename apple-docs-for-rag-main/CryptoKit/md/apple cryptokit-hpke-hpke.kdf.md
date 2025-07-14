

- Apple CryptoKit
- HPKE
-  HPKE.KDF 

Enumeration

# HPKE.KDF

The key derivation functions to use in HPKE.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
enum KDF
```

## Topics

### Enumeration Cases

case HKDF_SHA256

An HMAC-based key derivation function that uses SHA-2 hashing with a 256-bit digest.

case HKDF_SHA384

An HMAC-based key derivation function that uses SHA-2 hashing with a 384-bit digest.

case HKDF_SHA512

An HMAC-based key derivation function that uses SHA-2 hashing with a 512-bit digest.

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

enum KEM

The key encapsulation mechanisms to use in HPKE.

enum DHKEM

A container for Diffie-Hellman key encapsulation mechanisms (KEMs).

