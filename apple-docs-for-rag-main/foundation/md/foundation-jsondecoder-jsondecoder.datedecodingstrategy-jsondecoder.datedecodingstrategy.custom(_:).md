

- Foundation
- JSONDecoder
- JSONDecoder.DateDecodingStrategy
-  JSONDecoder.DateDecodingStrategy.custom(\_:) 

Case

# JSONDecoder.DateDecodingStrategy.custom(\_:)

The strategy that formats custom dates by calling a user-defined function.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
@preconcurrency
case custom((any Decoder) throws -> Date)
```

## See Also

### Custom Formats

case formatted(DateFormatter)

The strategy that defers formatting settings to a supplied date formatter.

