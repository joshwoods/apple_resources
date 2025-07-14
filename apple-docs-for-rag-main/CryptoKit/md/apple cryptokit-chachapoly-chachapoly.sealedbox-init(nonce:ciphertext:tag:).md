

- Apple CryptoKit
- ChaChaPoly
- ChaChaPoly.SealedBox
-  init(nonce:ciphertext:tag:) 

Initializer

# init(nonce:ciphertext:tag:)

Creates a sealed box from the given tag, nonce, and ciphertext.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
init(
    nonce: ChaChaPoly.Nonce,
    ciphertext: C,
    tag: T
) throws where C : DataProtocol, T : DataProtocol
```

## Parameters 

`nonce`  

The nonce.

`ciphertext`  

The encrypted data.

`tag`  

An authentication tag.

## See Also

### Creating the sealed box

init&lt;D>(combined: D) throws

Creates a sealed box from the given data.

