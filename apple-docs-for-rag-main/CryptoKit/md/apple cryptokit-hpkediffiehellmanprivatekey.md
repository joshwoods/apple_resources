

- Apple CryptoKit
-  HPKEDiffieHellmanPrivateKey 

Protocol

# HPKEDiffieHellmanPrivateKey

A type that represents the private key in a Diffie-Hellman key exchange.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
@preconcurrency
protocol HPKEDiffieHellmanPrivateKey : DiffieHellmanKeyAgreement where Self.PublicKey : HPKEDiffieHellmanPublicKey
```

## Relationships

### Inherits From

- DiffieHellmanKeyAgreement
- Sendable

### Inherited By

- HPKEDiffieHellmanPrivateKeyGeneration

### Conforming Types

- Curve25519.KeyAgreement.PrivateKey
- P256.KeyAgreement.PrivateKey
- P384.KeyAgreement.PrivateKey
- P521.KeyAgreement.PrivateKey
- SecureEnclave.P256.KeyAgreement.PrivateKey

