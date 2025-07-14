

- Apple CryptoKit
- SymmetricKey
-  init(data:) 

Initializer

# init(data:)

Creates a key from the given data.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
init(data: D) where D : ContiguousBytes
```

## Parameters 

`data`  

The contiguous bytes from which to create the key.

## See Also

### Creating a key

init(size: SymmetricKeySize)

Generates a new random key of the given size.

