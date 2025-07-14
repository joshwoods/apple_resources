

- Apple CryptoKit
- AES
- AES.GCM
- AES.GCM.SealedBox
-  init(nonce:ciphertext:tag:) 

Initializer

# init(nonce:ciphertext:tag:)

Creates a sealed box from the given tag, nonce, and ciphertext.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
init(
    nonce: AES.GCM.Nonce,
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

The authentication tag.

## See Also

### Creating the sealed box

init&lt;D>(combined: D) throws

Creates a sealed box from the combined bytes of an authentication tag, nonce, and encrypted data.

