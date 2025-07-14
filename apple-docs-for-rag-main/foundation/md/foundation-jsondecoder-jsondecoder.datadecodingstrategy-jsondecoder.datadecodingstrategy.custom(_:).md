

- Foundation
- JSONDecoder
- JSONDecoder.DataDecodingStrategy
-  JSONDecoder.DataDecodingStrategy.custom(\_:) 

Case

# JSONDecoder.DataDecodingStrategy.custom(\_:)

The strategy that decodes data using a user-defined function.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
@preconcurrency
case custom((any Decoder) throws -> Data)
```

