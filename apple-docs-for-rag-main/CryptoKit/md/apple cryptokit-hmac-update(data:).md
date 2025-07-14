

- Apple CryptoKit
- HMAC
-  update(data:) 

Instance Method

# update(data:)

Updates the message authentication code computation with a block of data.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
mutating func update(data: D) where D : DataProtocol
```

## Parameters 

`data`  

The data for which to compute the authentication code.

## See Also

### Creating an authentication code iteratively

init(key: SymmetricKey)

Creates a message authentication code generator.

func finalize() -> HMAC&lt;H>.MAC

Finalizes the message authentication computation and returns the computed code.

