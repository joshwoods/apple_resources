

- Apple CryptoKit
-  HPKEDiffieHellmanPrivateKeyGeneration 

Protocol

# HPKEDiffieHellmanPrivateKeyGeneration

A type that represents the generation of private keys in a Diffie-Hellman key exchange.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
@preconcurrency
protocol HPKEDiffieHellmanPrivateKeyGeneration : HPKEDiffieHellmanPrivateKey
```

## Topics

### Initializers

init()

Creates a private key generator.

**Required**

## Relationships

### Inherits From

- DiffieHellmanKeyAgreement
- HPKEDiffieHellmanPrivateKey
- Sendable

### Conforming Types

- Curve25519.KeyAgreement.PrivateKey
- P256.KeyAgreement.PrivateKey
- P384.KeyAgreement.PrivateKey
- P521.KeyAgreement.PrivateKey

