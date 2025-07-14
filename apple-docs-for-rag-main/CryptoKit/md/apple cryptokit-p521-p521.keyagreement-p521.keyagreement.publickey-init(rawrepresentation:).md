

- Apple CryptoKit
- P521
- P521.KeyAgreement
- P521.KeyAgreement.PublicKey
-  init(rawRepresentation:) 

Initializer

# init(rawRepresentation:)

Creates a P-521 public key for key agreement from a collection of bytes.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
init(rawRepresentation: D) throws where D : ContiguousBytes
```

## Parameters 

`rawRepresentation`  

A raw representation of the key as a collection of contiguous bytes.

## See Also

### Creating a public key

init&lt;Bytes>(compactRepresentation: Bytes) throws

Creates a P-521 public key for key agreement from a compact representation of the key.

init&lt;Bytes>(derRepresentation: Bytes) throws

Creates a P-521 public key for key agreement from a Distinguished Encoding Rules (DER) encoded representation.

init(pemRepresentation: String) throws

Creates a P-521 public key for key agreement from a Privacy-Enhanced Mail (PEM) representation.

init&lt;Bytes>(x963Representation: Bytes) throws

Creates a P-521 public key for key agreement from an ANSI x9.63 representation.

init&lt;Bytes>(compressedRepresentation: Bytes) throws

Creates a P-521 public key for key agreement from a compressed representation of the key.

