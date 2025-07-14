

- Apple CryptoKit
- P384
- P384.KeyAgreement
- P384.KeyAgreement.PrivateKey
-  x963Representation 

Instance Property

# x963Representation

An ANSI x9.63 representation of the private key.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
var x963Representation: Data { get }
```

## See Also

### Representing the key

var rawRepresentation: Data

A data representation of the private key.

var derRepresentation: Data

A Distinguished Encoding Rules (DER) encoded representation of the private key.

var pemRepresentation: String

A Privacy-Enhanced Mail (PEM) representation of the private key.

