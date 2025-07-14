

- Foundation
- JSONDecoder
- JSONDecoder.NonConformingFloatDecodingStrategy
-  JSONDecoder.NonConformingFloatDecodingStrategy.convertFromString(positiveInfinity:negativeInfinity:nan:) 

Case

# JSONDecoder.NonConformingFloatDecodingStrategy.convertFromString(positiveInfinity:negativeInfinity:nan:)

The strategy that decodes exceptional floating-point values from a specified string representation.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
case convertFromString(
    positiveInfinity: String,
    negativeInfinity: String,
    nan: String
)
```

## See Also

### Exceptional Values

case `throw`

The strategy that throws an error upon decoding an exceptional floating-point value.

