

- Apple CryptoKit
- ChaChaPoly
- ChaChaPoly.SealedBox
-  tag 

Instance Property

# tag

An authentication tag.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
var tag: Data { get }
```

## Discussion

The authentication tag has a length of 16 bytes.

## See Also

### Inspecting the component elements

var nonce: ChaChaPoly.Nonce

The nonce used to encrypt the data.

var ciphertext: Data

The encrypted data.

