

- Apple CryptoKit
- P521
- P521.KeyAgreement
- P521.KeyAgreement.PublicKey
-  derRepresentation 

Instance Property

# derRepresentation

A Distinguished Encoding Rules (DER) encoded representation of the public key.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
var derRepresentation: Data { get }
```

## See Also

### Representing the key

var rawRepresentation: Data

A full representation of the public key.

var compactRepresentation: Data?

A compact representation of the public key.

var pemRepresentation: String

A Privacy-Enhanced Mail (PEM) representation of the public key.

var x963Representation: Data

An ANSI x9.63 representation of the public key.

var compressedRepresentation: Data

A compressed representation of the public key.

