

- Apple CryptoKit
- P521
- P521.Signing
-  P521.Signing.PrivateKey 

Structure

# P521.Signing.PrivateKey

A P-521 private key used to create cryptographic signatures.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
struct PrivateKey
```

## Topics

### Creating a key

init&lt;Bytes>(rawRepresentation: Bytes) throws

Creates a P-521 private key for signing from a collection of bytes.

init(compactRepresentable: Bool)

Creates a random P-521 private key for signing.

init&lt;Bytes>(derRepresentation: Bytes) throws

Creates a P-521 private key for signing from a Distinguished Encoding Rules (DER) encoded representation.

init(pemRepresentation: String) throws

Creates a P-521 private key for signing from a Privacy-Enhanced Mail PEM) representation.

init&lt;Bytes>(x963Representation: Bytes) throws

Creates a P-521 private key for signing from an ANSI x9.63 representation.

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

var publicKey: P521.Signing.PublicKey

The corresponding public key.

### Creating a signature

func signature&lt;D>(for: D) throws -> P521.Signing.ECDSASignature

Generates an Elliptic Curve Digital Signature Algorithm (ECDSA) signature of the data you provide over the P-521 elliptic curve, using SHA-512 as the hash function.

func signature&lt;D>(for: D) throws -> P521.Signing.ECDSASignature

Generates an Elliptic Curve Digital Signature Algorithm (ECDSA) signature of the digest you provide over the P-521 elliptic curve.

struct ECDSASignature

A P-521 elliptic curve digital signature algorithm (ECDSA) signature.

## Relationships

### Conforms To

- Sendable

## See Also

### Using keys

struct PublicKey

A P-521 public key used to verify cryptographic signatures.

