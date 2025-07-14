

- Apple CryptoKit
- P384
- P384.Signing
- P384.Signing.PrivateKey
-  derRepresentation 

Instance Property

# derRepresentation

A Distinguished Encoding Rules (DER) encoded representation of the private key.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
var derRepresentation: Data { get }
```

## See Also

### Representing the key

var rawRepresentation: Data

A data representation of the private key.

var pemRepresentation: String

A Privacy-Enhanced Mail (PEM) representation of the private key.

var x963Representation: Data

An ANSI x9.63 representation of the private key.

