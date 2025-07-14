

- Apple CryptoKit
- P384
- P384.Signing
- P384.Signing.PrivateKey
-  init(x963Representation:) 

Initializer

# init(x963Representation:)

Creates a P-384 private key for signing from an ANSI x9.63 representation.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
init(x963Representation: Bytes) throws where Bytes : ContiguousBytes
```

## Parameters 

`x963Representation`  

An ANSI x9.63 representation of the key.

## See Also

### Creating a private key

init&lt;Bytes>(rawRepresentation: Bytes) throws

Creates a P-384 private key for signing from a collection of bytes.

init(compactRepresentable: Bool)

Creates a random P-384 private key for signing.

init&lt;Bytes>(derRepresentation: Bytes) throws

Creates a P-384 private key for signing from a Distinguished Encoding Rules (DER) encoded representation.

init(pemRepresentation: String) throws

Creates a P-384 private key for signing from a Privacy-Enhanced Mail PEM) representation.

