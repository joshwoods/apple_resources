

- Apple CryptoKit
- P521
- P521.Signing
-  P521.Signing.ECDSASignature 

Structure

# P521.Signing.ECDSASignature

A P-521 elliptic curve digital signature algorithm (ECDSA) signature.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
struct ECDSASignature
```

## Topics

### Creating a signature

init&lt;D>(derRepresentation: D) throws

Creates a P-521 digital signature from a Distinguished Encoding Rules (DER) encoded representation.

init&lt;D>(rawRepresentation: D) throws

Creates a P-521 digital signature from a raw representation.

### Representing the signature

var derRepresentation: Data

A Distinguished Encoding Rules (DER) encoded representation of a P-521 digital signature.

var rawRepresentation: Data

A raw data representation of a P-521 digital signature.

## Relationships

### Conforms To

- ContiguousBytes
- Sendable

## See Also

### Creating a signature

func signature&lt;D>(for: D) throws -> P521.Signing.ECDSASignature

Generates an Elliptic Curve Digital Signature Algorithm (ECDSA) signature of the data you provide over the P-521 elliptic curve, using SHA-512 as the hash function.

func signature&lt;D>(for: D) throws -> P521.Signing.ECDSASignature

Generates an Elliptic Curve Digital Signature Algorithm (ECDSA) signature of the digest you provide over the P-521 elliptic curve.

