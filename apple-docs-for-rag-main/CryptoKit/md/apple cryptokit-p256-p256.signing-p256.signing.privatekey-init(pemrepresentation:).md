

- Apple CryptoKit
- P256
- P256.Signing
- P256.Signing.PrivateKey
-  init(pemRepresentation:) 

Initializer

# init(pemRepresentation:)

Creates a P-256 private key for signing from a Privacy-Enhanced Mail PEM) representation.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
init(pemRepresentation: String) throws
```

## Parameters 

`pemRepresentation`  

A PEM representation of the key.

## See Also

### Creating a private key

init&lt;Bytes>(rawRepresentation: Bytes) throws

Creates a P-256 private key for signing from a collection of bytes.

init(compactRepresentable: Bool)

Creates a random P-256 private key for signing.

init&lt;Bytes>(derRepresentation: Bytes) throws

Creates a P-256 private key for signing from a Distinguished Encoding Rules (DER) encoded representation.

init&lt;Bytes>(x963Representation: Bytes) throws

Creates a P-256 private key for signing from an ANSI x9.63 representation.

