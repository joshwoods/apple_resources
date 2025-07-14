

- Apple CryptoKit
- P384
- P384.Signing
-  P384.Signing.PublicKey 

Structure

# P384.Signing.PublicKey

A P-384 public key used to verify cryptographic signatures.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
struct PublicKey
```

## Topics

### Creating a key

init&lt;D>(rawRepresentation: D) throws

Creates a P-384 public key for signing from a collection of bytes.

init&lt;Bytes>(compactRepresentation: Bytes) throws

Creates a P-384 public key for signing from a compact representation of the key.

init&lt;Bytes>(compressedRepresentation: Bytes) throws

Creates a P-384 public key for signing from a compressed representation of the key.

init&lt;Bytes>(derRepresentation: Bytes) throws

Creates a P-384 public key for signing from a Distinguished Encoding Rules (DER) encoded representation.

init(pemRepresentation: String) throws

Creates a P-384 public key for signing from a Privacy-Enhanced Mail (PEM) representation.

init&lt;Bytes>(x963Representation: Bytes) throws

Creates a P-384 public key for signing from an ANSI x9.63 representation.

### Representing the key

var rawRepresentation: Data

A full representation of the public key.

var compactRepresentation: Data?

A compact representation of the public key.

var compressedRepresentation: Data

A compressed representation of the public key.

var derRepresentation: Data

A Distinguished Encoding Rules (DER) encoded representation of the public key.

var pemRepresentation: String

A Privacy-Enhanced Mail (PEM) representation of the public key.

var x963Representation: Data

An ANSI x9.63 representation of the public key.

### Verifying a signature

func isValidSignature&lt;D>(P384.Signing.ECDSASignature, for: D) -> Bool

Verifies an elliptic curve digital signature algorithm (ECDSA) signature on a block of data over the P-384 elliptic curve.

func isValidSignature&lt;D>(P384.Signing.ECDSASignature, for: D) -> Bool

Verifies an elliptic curve digital signature algorithm (ECDSA) signature on a digest over the P-384 elliptic curve.

struct ECDSASignature

A P-384 elliptic curve digital signature algorithm (ECDSA) signature.

## Relationships

### Conforms To

- Sendable

## See Also

### Using keys

struct PrivateKey

A P-384 private key used to create cryptographic signatures.

