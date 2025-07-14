

- Apple CryptoKit
- P521
- P521.KeyAgreement
-  P521.KeyAgreement.PublicKey 

Structure

# P521.KeyAgreement.PublicKey

A P-521 public key used for key agreement.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
struct PublicKey
```

## Topics

### Creating a public key

init&lt;D>(rawRepresentation: D) throws

Creates a P-521 public key for key agreement from a collection of bytes.

init&lt;Bytes>(compactRepresentation: Bytes) throws

Creates a P-521 public key for key agreement from a compact representation of the key.

init&lt;Bytes>(derRepresentation: Bytes) throws

Creates a P-521 public key for key agreement from a Distinguished Encoding Rules (DER) encoded representation.

init(pemRepresentation: String) throws

Creates a P-521 public key for key agreement from a Privacy-Enhanced Mail (PEM) representation.

init&lt;Bytes>(x963Representation: Bytes) throws

Creates a P-521 public key for key agreement from an ANSI x9.63 representation.

init&lt;Bytes>(compressedRepresentation: Bytes) throws

Creates a P-521 public key for key agreement from a compressed representation of the key.

### Representing the key

var rawRepresentation: Data

A full representation of the public key.

var compactRepresentation: Data?

A compact representation of the public key.

var derRepresentation: Data

A Distinguished Encoding Rules (DER) encoded representation of the public key.

var pemRepresentation: String

A Privacy-Enhanced Mail (PEM) representation of the public key.

var x963Representation: Data

An ANSI x9.63 representation of the public key.

var compressedRepresentation: Data

A compressed representation of the public key.

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

A P-521 private key used for key agreement.

