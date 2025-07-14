

- Apple CryptoKit
- AES
- AES.GCM
- AES.GCM.SealedBox
-  combined 

Instance Property

# combined

A combined element composed of the nonce, encrypted data, and authentication tag.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
var combined: Data? { get }
```

## Discussion

The combined representation is only available when the AES.GCM.Nonce size is the default size of 12 bytes. The data layout of the combined representation is nonce, ciphertext, then tag.

