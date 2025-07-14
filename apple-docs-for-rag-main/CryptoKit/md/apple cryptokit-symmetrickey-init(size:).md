

- Apple CryptoKit
- SymmetricKey
-  init(size:) 

Initializer

# init(size:)

Generates a new random key of the given size.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
init(size: SymmetricKeySize)
```

## Parameters 

`size`  

The size of the key to generate. You can use one of the standard sizes, like bits256, or you can create a key of custom length by initializing a SymmetricKeySize instance with a non-standard value.

## See Also

### Creating a key

init&lt;D>(data: D)

Creates a key from the given data.

