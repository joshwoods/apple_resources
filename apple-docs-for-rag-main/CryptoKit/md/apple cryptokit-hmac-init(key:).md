

- Apple CryptoKit
- HMAC
-  init(key:) 

Initializer

# init(key:)

Creates a message authentication code generator.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
init(key: SymmetricKey)
```

## Parameters 

`key`  

The symmetric key used to secure the computation.

## See Also

### Creating an authentication code iteratively

func update&lt;D>(data: D)

Updates the message authentication code computation with a block of data.

func finalize() -> HMAC&lt;H>.MAC

Finalizes the message authentication computation and returns the computed code.

