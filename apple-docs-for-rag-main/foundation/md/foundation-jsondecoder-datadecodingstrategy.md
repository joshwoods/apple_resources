

- Foundation
- JSONDecoder
-  dataDecodingStrategy 

Instance Property

# dataDecodingStrategy

The strategy that a decoder uses to decode raw data.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var dataDecodingStrategy: JSONDecoder.DataDecodingStrategy { get set }
```

## Discussion

The default strategy is the JSONDecoder.DataDecodingStrategy.base64 strategy.

## See Also

### Decoding Raw Data

enum DataDecodingStrategy

The strategies for decoding raw data.

