

- Apple CryptoKit
- ChaChaPoly
- ChaChaPoly.SealedBox
-  init(combined:) 

Initializer

# init(combined:)

Creates a sealed box from the given data.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
init(combined: D) throws where D : DataProtocol
```

## Parameters 

`combined`  

The combined bytes of the tag and ciphertext.

## See Also

### Creating the sealed box

init&lt;C, T>(nonce: ChaChaPoly.Nonce, ciphertext: C, tag: T) throws

Creates a sealed box from the given tag, nonce, and ciphertext.

