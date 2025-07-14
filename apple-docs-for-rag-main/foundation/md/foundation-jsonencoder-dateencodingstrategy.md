

- Foundation
- JSONEncoder
-  dateEncodingStrategy 

Instance Property

# dateEncodingStrategy

The strategy used when encoding dates as part of a JSON object.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var dateEncodingStrategy: JSONEncoder.DateEncodingStrategy { get set }
```

## Discussion

The default strategy is the JSONEncoder.DateEncodingStrategy.deferredToDate strategy.

## See Also

### Encoding Dates

enum DateEncodingStrategy

The formatting strategies available for formatting dates when encoding a date as JSON.

