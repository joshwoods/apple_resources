

- Apple CryptoKit
- P256
- P256.Signing
- P256.Signing.PrivateKey
-  rawRepresentation 

Instance Property

# rawRepresentation

A data representation of the private key.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
var rawRepresentation: Data { get }
```

## See Also

### Representing the key

var derRepresentation: Data

A Distinguished Encoding Rules (DER) encoded representation of the private key.

var pemRepresentation: String

A Privacy-Enhanced Mail (PEM) representation of the private key.

var x963Representation: Data

An ANSI x9.63 representation of the private key.

