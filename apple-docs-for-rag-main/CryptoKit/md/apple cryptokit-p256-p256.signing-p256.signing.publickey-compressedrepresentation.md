

- Apple CryptoKit
- P256
- P256.Signing
- P256.Signing.PublicKey
-  compressedRepresentation 

Instance Property

# compressedRepresentation

A compressed representation of the public key.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
var compressedRepresentation: Data { get }
```

## See Also

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

