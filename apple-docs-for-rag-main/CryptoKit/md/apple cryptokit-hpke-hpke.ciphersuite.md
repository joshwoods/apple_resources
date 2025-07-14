

- Apple CryptoKit
- HPKE
-  HPKE.Ciphersuite 

Structure

# HPKE.Ciphersuite

Cipher suites to use in hybrid public key encryption.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
struct Ciphersuite
```

## Overview

HPKE cipher suites identify the authenticated encryption with additional data (AEAD) algorithm for encrypting and decrypting messages, the key derivation function (KDF) for deriving the shared key, and the key encapsulation mechanism (KEM) for sharing the symmetric key. The sender and recipient of encrypted messages need to use the same cipher suite.

## Topics

### Initializers

init(kem: HPKE.KEM, kdf: HPKE.KDF, aead: HPKE.AEAD)

Creates an HPKE cipher suite.

### Instance Properties

let aead: HPKE.AEAD

The authenticated encryption with additional data (AEAD) algorithm for encrypting and decrypting messages.

let kdf: HPKE.KDF

The key derivation function (KDF) for deriving the symmetric key.

let kem: HPKE.KEM

The key encapsulation mechanism (KEM) for encapsulating the symmetric key.

### Type Properties

static let Curve25519_SHA256_ChachaPoly: HPKE.Ciphersuite

A cipher suite for HPKE that uses X25519 elliptic curve key agreement, SHA-2 key derivation with a 256-bit digest, and the ChaCha20 stream cipher with the Poly1305 message authentication code.

static let P256_SHA256_AES_GCM_256: HPKE.Ciphersuite

A cipher suite for HPKE that uses NIST P-256 elliptic curve key agreement, SHA-2 key derivation with a 256-bit digest, and the Advanced Encryption Standard cipher in Galois/Counter Mode with a key length of 256 bits.

static let P384_SHA384_AES_GCM_256: HPKE.Ciphersuite

A cipher suite that you use for HPKE using NIST P-384 elliptic curve key agreement, SHA-2 key derivation with a 384-bit digest, and the Advanced Encryption Standard cipher in Galois/Counter Mode with a key length of 256 bits.

static let P521_SHA512_AES_GCM_256: HPKE.Ciphersuite

A cipher suite for HPKE that uses NIST P-521 elliptic curve key agreement, SHA-2 key derivation with a 512-bit digest, and the Advanced Encryption Standard cipher in Galois/Counter Mode with a key length of 256 bits.

## Relationships

### Conforms To

- Sendable

## See Also

### Choosing cryptographic algorithms

enum AEAD

The authenticated encryption with associated data (AEAD) algorithms to use in HPKE.

enum KDF

The key derivation functions to use in HPKE.

enum KEM

The key encapsulation mechanisms to use in HPKE.

enum DHKEM

A container for Diffie-Hellman key encapsulation mechanisms (KEMs).

