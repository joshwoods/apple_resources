

- Apple CryptoKit
- SymmetricKeySize
-  init(bitCount:) 

Initializer

# init(bitCount:)

Creates a new key size of the given length.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
init(bitCount: Int)
```

## Parameters 

`bitCount`  

The number of bits in the key size.

## Discussion

In most cases, you can use one of the standard key sizes, like bits256. If instead you need a key with a non-standard size, use the init(bitCount:) initializer to create a custom key size.

