

- Foundation
- PropertyListEncoder
-  init() 

Initializer

# init()

Creates a new, reusable property list encoder with the default formatting settings.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init()
```

## See Also

### Encoding

func encode&lt;Value>(Value) throws -> Data

Returns a property list that represents an encoded version of the value you supply.

func encode&lt;T, C>(T, configuration: C.Type) throws -> Data

func encode&lt;T>(T, configuration: T.EncodingConfiguration) throws -> Data

