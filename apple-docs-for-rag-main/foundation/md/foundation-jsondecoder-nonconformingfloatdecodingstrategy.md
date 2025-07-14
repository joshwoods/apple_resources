

- Foundation
- JSONDecoder
-  nonConformingFloatDecodingStrategy 

Instance Property

# nonConformingFloatDecodingStrategy

The strategy used by a decoder when it encounters exceptional floating-point values.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var nonConformingFloatDecodingStrategy: JSONDecoder.NonConformingFloatDecodingStrategy { get set }
```

## Discussion

The default strategy is the JSONDecoder.NonConformingFloatDecodingStrategy.throw strategy.

## See Also

### Decoding Exceptional Numbers

enum NonConformingFloatDecodingStrategy

The strategies for encoding nonconforming floating-point numbers, also known as IEEE 754 exceptional values.

