

- Apple CryptoKit
- HPKE
-  HPKE.AEAD 

Enumeration

# HPKE.AEAD

The authenticated encryption with associated data (AEAD) algorithms to use in HPKE.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
enum AEAD
```

## Topics

### Enumeration Cases

case AES_GCM_128

An Advanced Encryption Standard cipher in Galois/Counter Mode with a key length of 128 bits.

case AES_GCM_256

An Advanced Encryption Standard cipher in Galois/Counter Mode with a key length of 256 bits.

case chaChaPoly

A ChaCha20 stream cipher with the Poly1305 message authentication code.

case exportOnly

An export-only mode.

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

enum KDF

The key derivation functions to use in HPKE.

enum KEM

The key encapsulation mechanisms to use in HPKE.

enum DHKEM

A container for Diffie-Hellman key encapsulation mechanisms (KEMs).

