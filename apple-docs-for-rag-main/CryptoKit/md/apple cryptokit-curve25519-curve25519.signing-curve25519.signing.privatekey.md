

- Apple CryptoKit
- Curve25519
- Curve25519.Signing
-  Curve25519.Signing.PrivateKey 

Structure

# Curve25519.Signing.PrivateKey

A Curve25519 private key used to create cryptographic signatures.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
struct PrivateKey
```

## Topics

### Creating a private key

init()

Creates a random Curve25519 private key for signing.

init&lt;D>(rawRepresentation: D) throws

Creates a Curve25519 private key for signing from a data representation.

### Reporting the private key

var rawRepresentation: Data

The raw representation of the key as a collection of contiguous bytes.

### Finding the public key

var publicKey: Curve25519.Signing.PublicKey

The corresponding public key.

### Creating a signature

func signature&lt;D>(for: D) throws -> Data

Generates an EdDSA signature over Curve25519.

## Relationships

### Conforms To

- Sendable

## See Also

### Using keys

struct PublicKey

A Curve25519 public key used to verify cryptographic signatures.

