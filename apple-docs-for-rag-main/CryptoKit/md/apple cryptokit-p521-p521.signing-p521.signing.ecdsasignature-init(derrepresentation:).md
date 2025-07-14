

- Apple CryptoKit
- P521
- P521.Signing
- P521.Signing.ECDSASignature
-  init(derRepresentation:) 

Initializer

# init(derRepresentation:)

Creates a P-521 digital signature from a Distinguished Encoding Rules (DER) encoded representation.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
init(derRepresentation: D) throws where D : DataProtocol
```

## Parameters 

`derRepresentation`  

The DER-encoded representation of the signature.

## See Also

### Creating a signature

init&lt;D>(rawRepresentation: D) throws

Creates a P-521 digital signature from a raw representation.

