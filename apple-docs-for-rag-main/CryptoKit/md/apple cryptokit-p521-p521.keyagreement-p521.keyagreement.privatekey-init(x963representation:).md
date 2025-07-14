

- Apple CryptoKit
- P521
- P521.KeyAgreement
- P521.KeyAgreement.PrivateKey
-  init(x963Representation:) 

Initializer

# init(x963Representation:)

Creates a P-521 private key for key agreement from an ANSI x9.63 representation.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
init(x963Representation: Bytes) throws where Bytes : ContiguousBytes
```

## Parameters 

`x963Representation`  

An ANSI x9.63 representation of the key.

## See Also

### Creating a private key

init(compactRepresentable: Bool)

Creates a random P-521 private key for key agreement.

init&lt;Bytes>(rawRepresentation: Bytes) throws

Creates a P-521 private key for key agreement from a collection of bytes.

init&lt;Bytes>(derRepresentation: Bytes) throws

Creates a P-521 private key for key agreement from a Distinguished Encoding Rules (DER) encoded representation.

init(pemRepresentation: String) throws

Creates a P-521 private key for key agreement from a Privacy-Enhanced Mail PEM) representation.

