

- Foundation
- JSONDecoder
- JSONDecoder.DateDecodingStrategy
-  JSONDecoder.DateDecodingStrategy.formatted(\_:) 

Case

# JSONDecoder.DateDecodingStrategy.formatted(\_:)

The strategy that defers formatting settings to a supplied date formatter.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
case formatted(DateFormatter)
```

## See Also

### Custom Formats

case custom((any Decoder) throws -> Date)

The strategy that formats custom dates by calling a user-defined function.

