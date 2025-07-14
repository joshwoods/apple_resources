

- Apple CryptoKit
- P521
- P521.Signing
- P521.Signing.ECDSASignature
-  init(rawRepresentation:) 

Initializer

# init(rawRepresentation:)

Creates a P-521 digital signature from a raw representation.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
init(rawRepresentation: D) throws where D : DataProtocol
```

## Parameters 

`rawRepresentation`  

A raw representation of the signature as a collection of contiguous bytes.

## See Also

### Creating a signature

init&lt;D>(derRepresentation: D) throws

Creates a P-521 digital signature from a Distinguished Encoding Rules (DER) encoded representation.

