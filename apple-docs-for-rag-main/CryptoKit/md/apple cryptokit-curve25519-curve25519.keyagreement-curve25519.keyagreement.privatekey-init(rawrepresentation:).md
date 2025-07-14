

- Apple CryptoKit
- Curve25519
- Curve25519.KeyAgreement
- Curve25519.KeyAgreement.PrivateKey
-  init(rawRepresentation:) 

Initializer

# init(rawRepresentation:)

Creates a Curve25519 private key for key agreement from a collection of bytes.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
init(rawRepresentation: D) throws where D : ContiguousBytes
```

## Parameters 

`rawRepresentation`  

A raw representation of the key as a collection of contiguous bytes.

## See Also

### Creating a private key

init()

Creates a random Curve25519 private key for key agreement.

