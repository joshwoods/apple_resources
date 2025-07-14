

- Apple CryptoKit
- SecureEnclave
- SecureEnclave.P256
- SecureEnclave.P256.Signing
-  SecureEnclave.P256.Signing.PrivateKey 

Structure

# SecureEnclave.P256.Signing.PrivateKey

A P-256 private key used for signing.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
struct PrivateKey
```

## Topics

### Creating a private key

init(dataRepresentation: Data) throws

Creates a P-256 private key for signing from the specified data representation.

init(dataRepresentation: Data, authenticationContext: LAContext?) throws

Creates a P-256 private key for signing from a data representation of the key with the given authentication context.

init(compactRepresentable: Bool, accessControl: SecAccessControl) throws

Creates a P-256 private key for signing with the specified access control.

init(compactRepresentable: Bool, accessControl: SecAccessControl, authenticationContext: LAContext?) throws

Creates a P-256 private key for signing with the specified access control.

### Representing the key

let dataRepresentation: Data

A data representation of the private key.

### Getting the public key

let publicKey: P256.Signing.PublicKey

The corresponding public key.

### Generating a signature

func signature&lt;D>(for: D) throws -> P256.Signing.ECDSASignature

Generates an Elliptic Curve Digital Signature Algorithm (ECDSA) signature of the digest you provide over the P-256 elliptic curve.

func signature&lt;D>(for: D) throws -> P256.Signing.ECDSASignature

Generates an elliptic curve digital signature algorithm (ECDSA) signature of the given data over the P-256 elliptic curve, using SHA-256 as the hash function.

## Relationships

### Conforms To

- Sendable

