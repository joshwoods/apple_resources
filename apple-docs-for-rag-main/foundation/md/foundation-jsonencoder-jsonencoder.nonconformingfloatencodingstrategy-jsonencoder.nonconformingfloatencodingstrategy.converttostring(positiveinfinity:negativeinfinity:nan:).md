

- Foundation
- JSONEncoder
- JSONEncoder.NonConformingFloatEncodingStrategy
-  JSONEncoder.NonConformingFloatEncodingStrategy.convertToString(positiveInfinity:negativeInfinity:nan:) 

Case

# JSONEncoder.NonConformingFloatEncodingStrategy.convertToString(positiveInfinity:negativeInfinity:nan:)

The strategy that encodes exceptional floating-point values from a specified string representation.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
case convertToString(
    positiveInfinity: String,
    negativeInfinity: String,
    nan: String
)
```

## See Also

### Exceptional Values

case `throw`

The strategy that throws an error upon encoding an exceptional floating-point value.

