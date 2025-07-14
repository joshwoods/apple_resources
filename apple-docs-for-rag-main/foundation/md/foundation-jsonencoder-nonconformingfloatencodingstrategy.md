

- Foundation
- JSONEncoder
-  nonConformingFloatEncodingStrategy 

Instance Property

# nonConformingFloatEncodingStrategy

The strategy used by an encoder when it encounters exceptional floating-point values.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var nonConformingFloatEncodingStrategy: JSONEncoder.NonConformingFloatEncodingStrategy { get set }
```

## Discussion

The default strategy is the JSONEncoder.NonConformingFloatEncodingStrategy.throw strategy.

## See Also

### Encoding Exceptional Numbers

enum NonConformingFloatEncodingStrategy

The strategies for encoding nonconforming floating-point numbers, also known as IEEE 754 exceptional values.

