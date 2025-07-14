

- Foundation
- JSONDecoder
-  dateDecodingStrategy 

Instance Property

# dateDecodingStrategy

The strategy used when decoding dates from part of a JSON object.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var dateDecodingStrategy: JSONDecoder.DateDecodingStrategy { get set }
```

## Discussion

The default strategy is the JSONDecoder.DateDecodingStrategy.deferredToDate strategy.

## See Also

### Decoding Dates

enum DateDecodingStrategy

The strategies available for formatting dates when decoding them from JSON.

