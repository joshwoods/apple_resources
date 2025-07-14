

- Apple CryptoKit
-  HPKEPublicKeySerialization 

Protocol

# HPKEPublicKeySerialization

A type that HPKE uses to encode the public key.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
@preconcurrency
protocol HPKEPublicKeySerialization : Sendable
```

## Topics

### Initializers

init&lt;D>(D, kem: HPKE.KEM) throws

Creates a public key from an encoded representation.

**Required**

### Instance Methods

func hpkeRepresentation(kem: HPKE.KEM) throws -> Data

Creates an encoded representation of the public key.

**Required**

## Relationships

### Inherits From

- Sendable

### Inherited By

- HPKEDiffieHellmanPublicKey

### Conforming Types

- Curve25519.KeyAgreement.PublicKey
- P256.KeyAgreement.PublicKey
- P384.KeyAgreement.PublicKey
- P521.KeyAgreement.PublicKey

