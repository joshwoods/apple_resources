

- Apple CryptoKit
- P256
- P256.KeyAgreement
- P256.KeyAgreement.PublicKey
-  init(pemRepresentation:) 

Initializer

# init(pemRepresentation:)

Creates a P-256 public key for key agreement from a Privacy-Enhanced Mail (PEM) representation.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
init(pemRepresentation: String) throws
```

## Parameters 

`pemRepresentation`  

A PEM representation of the key.

## See Also

### Creating a public key

init&lt;D>(rawRepresentation: D) throws

Creates a P-256 public key for key agreement from a collection of bytes.

init&lt;Bytes>(compactRepresentation: Bytes) throws

Creates a P-256 public key for key agreement from a compact representation of the key.

init&lt;Bytes>(derRepresentation: Bytes) throws

Creates a P-256 public key for key agreement from a Distinguished Encoding Rules (DER) encoded representation.

init&lt;Bytes>(x963Representation: Bytes) throws

Creates a P-256 public key for key agreement from an ANSI x9.63 representation.

init&lt;Bytes>(compressedRepresentation: Bytes) throws

Creates a P-256 public key for key agreement from a compressed representation of the key.

