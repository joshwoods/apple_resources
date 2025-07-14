

- Apple CryptoKit
- P384
- P384.Signing
- P384.Signing.PublicKey
-  init(x963Representation:) 

Initializer

# init(x963Representation:)

Creates a P-384 public key for signing from an ANSI x9.63 representation.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
init(x963Representation: Bytes) throws where Bytes : ContiguousBytes
```

## Parameters 

`x963Representation`  

An ANSI x9.63 representation of the key.

## See Also

### Creating a key

init&lt;D>(rawRepresentation: D) throws

Creates a P-384 public key for signing from a collection of bytes.

init&lt;Bytes>(compactRepresentation: Bytes) throws

Creates a P-384 public key for signing from a compact representation of the key.

init&lt;Bytes>(compressedRepresentation: Bytes) throws

Creates a P-384 public key for signing from a compressed representation of the key.

init&lt;Bytes>(derRepresentation: Bytes) throws

Creates a P-384 public key for signing from a Distinguished Encoding Rules (DER) encoded representation.

init(pemRepresentation: String) throws

Creates a P-384 public key for signing from a Privacy-Enhanced Mail (PEM) representation.

