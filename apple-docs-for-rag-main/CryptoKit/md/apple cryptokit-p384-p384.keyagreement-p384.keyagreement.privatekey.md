

- Apple CryptoKit
- P384
- P384.KeyAgreement
-  P384.KeyAgreement.PrivateKey 

Structure

# P384.KeyAgreement.PrivateKey

A P-384 private key used for key agreement.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
struct PrivateKey
```

## Topics

### Creating a private key

init&lt;Bytes>(rawRepresentation: Bytes) throws

Creates a P-384 private key for key agreement from a collection of bytes.

init(compactRepresentable: Bool)

Creates a random P-384 private key for key agreement.

init&lt;Bytes>(derRepresentation: Bytes) throws

Creates a P-384 private key for key agreement from a Distinguished Encoding Rules (DER) encoded representation.

init(pemRepresentation: String) throws

Creates a P-384 private key for key agreement from a Privacy-Enhanced Mail PEM) representation.

init&lt;Bytes>(x963Representation: Bytes) throws

Creates a P-384 private key for key agreement from an ANSI x9.63 representation.

### Representing the key

var rawRepresentation: Data

A data representation of the private key.

var derRepresentation: Data

A Distinguished Encoding Rules (DER) encoded representation of the private key.

var pemRepresentation: String

A Privacy-Enhanced Mail (PEM) representation of the private key.

var x963Representation: Data

An ANSI x9.63 representation of the private key.

### Finding the public key

var publicKey: P384.KeyAgreement.PublicKey

The corresponding public key.

### Creating a shared secret

func sharedSecretFromKeyAgreement(with: P384.KeyAgreement.PublicKey) throws -> SharedSecret

Computes a shared secret with the provided public key from another party.

struct SharedSecret

A key agreement result from which you can derive a symmetric cryptographic key.

### Default Implementations

DiffieHellmanKeyAgreement Implementations

HPKEDiffieHellmanPrivateKeyGeneration Implementations

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

A P-384 public key used for key agreement.

