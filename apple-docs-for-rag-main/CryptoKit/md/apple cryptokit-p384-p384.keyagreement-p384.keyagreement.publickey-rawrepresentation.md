

- Apple CryptoKit
- P384
- P384.KeyAgreement
- P384.KeyAgreement.PublicKey
-  rawRepresentation 

Instance Property

# rawRepresentation

A full representation of the public key.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
var rawRepresentation: Data { get }
```

## See Also

### Representing the key

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

