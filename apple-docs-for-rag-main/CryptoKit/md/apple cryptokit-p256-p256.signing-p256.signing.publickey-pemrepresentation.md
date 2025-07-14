

- Apple CryptoKit
- P256
- P256.Signing
- P256.Signing.PublicKey
-  pemRepresentation 

Instance Property

# pemRepresentation

A Privacy-Enhanced Mail (PEM) representation of the public key.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
var pemRepresentation: String { get }
```

## See Also

### Representing the key

var rawRepresentation: Data

A full representation of the public key.

var compactRepresentation: Data?

A compact representation of the public key.

var compressedRepresentation: Data

A compressed representation of the public key.

var derRepresentation: Data

A Distinguished Encoding Rules (DER) encoded representation of the public key.

var x963Representation: Data

An ANSI x9.63 representation of the public key.

