

- Apple CryptoKit
- Curve25519
- Curve25519.KeyAgreement
-  Curve25519.KeyAgreement.PrivateKey 

Structure

# Curve25519.KeyAgreement.PrivateKey

A Curve25519 private key used for key agreement.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
struct PrivateKey
```

## Topics

### Creating a private key

init()

Creates a random Curve25519 private key for key agreement.

init&lt;D>(rawRepresentation: D) throws

Creates a Curve25519 private key for key agreement from a collection of bytes.

### Reporting the private key

var rawRepresentation: Data

The raw representation of the key as a collection of contiguous bytes.

### Finding the public key

var publicKey: Curve25519.KeyAgreement.PublicKey

The corresponding public key.

### Creating a shared secret

func sharedSecretFromKeyAgreement(with: Curve25519.KeyAgreement.PublicKey) throws -> SharedSecret

Computes a shared secret with the provided public key from another party.

struct SharedSecret

A key agreement result from which you can derive a symmetric cryptographic key.

## Relationships

### Conforms To

- Copyable
- DiffieHellmanKeyAgreement
- HPKEDiffieHellmanPrivateKey
- HPKEDiffieHellmanPrivateKeyGeneration
- Sendable

## See Also

### Using keys

struct PublicKey

A Curve25519 public key used for key agreement.

