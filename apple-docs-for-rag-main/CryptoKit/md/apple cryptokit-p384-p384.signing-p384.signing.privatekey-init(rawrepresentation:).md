

- Apple CryptoKit
- P384
- P384.Signing
- P384.Signing.PrivateKey
-  init(rawRepresentation:) 

Initializer

# init(rawRepresentation:)

Creates a P-384 private key for signing from a collection of bytes.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
init(rawRepresentation: Bytes) throws where Bytes : ContiguousBytes
```

## Parameters 

`rawRepresentation`  

A raw representation of the key as a collection of contiguous bytes.

## See Also

### Creating a private key

init(compactRepresentable: Bool)

Creates a random P-384 private key for signing.

init&lt;Bytes>(derRepresentation: Bytes) throws

Creates a P-384 private key for signing from a Distinguished Encoding Rules (DER) encoded representation.

init(pemRepresentation: String) throws

Creates a P-384 private key for signing from a Privacy-Enhanced Mail PEM) representation.

init&lt;Bytes>(x963Representation: Bytes) throws

Creates a P-384 private key for signing from an ANSI x9.63 representation.

