

- Apple CryptoKit
- Curve25519
- Curve25519.Signing
- Curve25519.Signing.PublicKey
-  init(rawRepresentation:) 

Initializer

# init(rawRepresentation:)

Creates a Curve25519 public key from a data representation.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
init(rawRepresentation: D) throws where D : ContiguousBytes
```

## Parameters 

`rawRepresentation`  

A representation of the key as contiguous bytes from which to create the key.

