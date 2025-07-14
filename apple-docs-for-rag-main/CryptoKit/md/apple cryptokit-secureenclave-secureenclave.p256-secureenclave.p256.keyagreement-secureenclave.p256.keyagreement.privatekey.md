

- Apple CryptoKit
- SecureEnclave
- SecureEnclave.P256
- SecureEnclave.P256.KeyAgreement
-  SecureEnclave.P256.KeyAgreement.PrivateKey 

Structure

# SecureEnclave.P256.KeyAgreement.PrivateKey

A P-256 private key used for key agreement.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
struct PrivateKey
```

## Topics

### Creating a private key

init(dataRepresentation: Data) throws

Creates a P-256 private key for key agreement from the specified data representation.

init(dataRepresentation: Data, authenticationContext: LAContext?) throws

Creates a P-256 private key for key agreement from a data representation of the key with the given authentication context.

init(compactRepresentable: Bool, accessControl: SecAccessControl) throws

Creates a P-256 private key for key agreement with the specified access control.

init(compactRepresentable: Bool, accessControl: SecAccessControl, authenticationContext: LAContext?) throws

Creates a P-256 private key for key agreement with the specified access control.

### Representing the key

let dataRepresentation: Data

A data representation of the private key.

### Finding the public key

let publicKey: P256.KeyAgreement.PublicKey

The corresponding public key.

### Creating a shared secret

func sharedSecretFromKeyAgreement(with: P256.KeyAgreement.PublicKey) throws -> SharedSecret

Computes a shared secret with the provided public key from another party.

struct SharedSecret

A key agreement result from which you can derive a symmetric cryptographic key.

### Default Implementations

DiffieHellmanKeyAgreement Implementations

## Relationships

### Conforms To

- Copyable
- DiffieHellmanKeyAgreement
- HPKEDiffieHellmanPrivateKey
- Sendable

