

- Apple CryptoKit
-  HPKEDiffieHellmanPublicKey 

Protocol

# HPKEDiffieHellmanPublicKey

A type that represents the public key in a Diffie-Hellman key exchange.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
@preconcurrency
protocol HPKEDiffieHellmanPublicKey : HPKEPublicKeySerialization
```

## Topics

### Associated Types

associatedtype EphemeralPrivateKey : HPKEDiffieHellmanPrivateKeyGeneration

The type of the ephemeral private key.

**Required**

## Relationships

### Inherits From

- HPKEPublicKeySerialization
- Sendable

### Conforming Types

- Curve25519.KeyAgreement.PublicKey
- P256.KeyAgreement.PublicKey
- P384.KeyAgreement.PublicKey
- P521.KeyAgreement.PublicKey

