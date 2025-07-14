

- Apple CryptoKit
- AES
- AES.GCM
- AES.GCM.SealedBox
-  ciphertext 

Instance Property

# ciphertext

The encrypted data.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
var ciphertext: Data { get }
```

## Discussion

The length of the ciphertext of a sealed box is the same as the length of the plaintext you encrypt.

## See Also

### Inspecting the component elements

var nonce: AES.GCM.Nonce

The nonce used to encrypt the data.

var tag: Data

An authentication tag.

