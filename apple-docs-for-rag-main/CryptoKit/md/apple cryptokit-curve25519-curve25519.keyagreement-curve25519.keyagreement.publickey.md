

- Apple CryptoKit
- Curve25519
- Curve25519.KeyAgreement
-  Curve25519.KeyAgreement.PublicKey 

Structure

# Curve25519.KeyAgreement.PublicKey

A Curve25519 public key used for key agreement.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
struct PublicKey
```

## Topics

### Creating a public key

init&lt;D>(rawRepresentation: D) throws

Creates a Curve25519 public key for key agreement from a collection of bytes.

### Representing the key

var rawRepresentation: Data

A representation of the Curve25519 public key as a collection of bytes.

### Type Aliases

typealias HPKEEphemeralPrivateKey

The type of the ephemeral private key associated with this public key.

### Default Implementations

HPKEDiffieHellmanPublicKey Implementations

HPKEPublicKeySerialization Implementations

## Relationships

### Conforms To

- Copyable
- HPKEDiffieHellmanPublicKey
- HPKEPublicKeySerialization
- Sendable

## See Also

### Using keys

struct PrivateKey

A Curve25519 private key used for key agreement.

