

- Foundation
- JSONEncoder
- JSONEncoder.KeyEncodingStrategy
-  JSONEncoder.KeyEncodingStrategy.useDefaultKeys 

Case

# JSONEncoder.KeyEncodingStrategy.useDefaultKeys

A key encoding strategy that doesn’t change key names during encoding.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
case useDefaultKeys
```

## Discussion

The JSONEncoder.KeyEncodingStrategy.useDefaultKeys strategy is the strategy used if you don’t specify one.

Note

If you use a nested `CodingKeys` enumeration to define custom key names, this strategy continues to use those names rather than reverting back to the original property names. Nested `CodingKeys` enumerations are described in Encoding and Decoding Custom Types.

## See Also

### Built-in Encoding

case convertToSnakeCase

A key encoding strategy that converts camel-case keys to snake-case keys.

