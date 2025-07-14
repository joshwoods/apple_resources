

- Apple CryptoKit
- Curve25519
- Curve25519.Signing
-  Curve25519.Signing.PublicKey 

Structure

# Curve25519.Signing.PublicKey

A Curve25519 public key used to verify cryptographic signatures.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
struct PublicKey
```

## Topics

### Creating a public key

init&lt;D>(rawRepresentation: D) throws

Creates a Curve25519 public key from a data representation.

### Representing the key

var rawRepresentation: Data

A representation of the public key.

### Verifying a signature

func isValidSignature&lt;S, D>(S, for: D) -> Bool

Verifies an EdDSA signature over Curve25519.

## Relationships

### Conforms To

- Sendable

## See Also

### Using keys

struct PrivateKey

A Curve25519 private key used to create cryptographic signatures.

