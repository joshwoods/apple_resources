

- Apple CryptoKit
- ChaChaPoly
- ChaChaPoly.SealedBox
-  combined 

Instance Property

# combined

A combined element composed of the tag, the nonce, and the ciphertext.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
let combined: Data
```

## Discussion

The data layout of the combined representation is: nonce, ciphertext, then tag.

