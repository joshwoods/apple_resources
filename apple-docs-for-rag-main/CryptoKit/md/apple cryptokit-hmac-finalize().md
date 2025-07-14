

- Apple CryptoKit
- HMAC
-  finalize() 

Instance Method

# finalize()

Finalizes the message authentication computation and returns the computed code.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func finalize() -> HMAC.MAC
```

## Return Value

The message authentication code.

## See Also

### Creating an authentication code iteratively

init(key: SymmetricKey)

Creates a message authentication code generator.

func update&lt;D>(data: D)

Updates the message authentication code computation with a block of data.

