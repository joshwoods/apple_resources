

- Apple CryptoKit
- P256
- P256.KeyAgreement
- P256.KeyAgreement.PrivateKey
-  init(derRepresentation:) 

Initializer

# init(derRepresentation:)

Creates a P-256 private key for key agreement from a Distinguished Encoding Rules (DER) encoded representation.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
init(derRepresentation: Bytes) throws where Bytes : RandomAccessCollection, Bytes.Element == UInt8
```

## Parameters 

`derRepresentation`  

A DER-encoded representation of the key.

## See Also

### Creating a private key

init&lt;Bytes>(rawRepresentation: Bytes) throws

Creates a P-256 private key for key agreement from a collection of bytes.

init(compactRepresentable: Bool)

Creates a random P-256 private key for key agreement.

init(pemRepresentation: String) throws

Creates a P-256 private key for key agreement from a Privacy-Enhanced Mail PEM) representation.

init&lt;Bytes>(x963Representation: Bytes) throws

Creates a P-256 private key for key agreement from an ANSI x9.63 representation.

