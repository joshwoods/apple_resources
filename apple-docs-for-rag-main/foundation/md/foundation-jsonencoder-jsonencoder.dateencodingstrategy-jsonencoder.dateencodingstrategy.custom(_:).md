

- Foundation
- JSONEncoder
- JSONEncoder.DateEncodingStrategy
-  JSONEncoder.DateEncodingStrategy.custom(\_:) 

Case

# JSONEncoder.DateEncodingStrategy.custom(\_:)

The strategy that formats custom dates by calling a user-defined function.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
@preconcurrency
case custom((Date, any Encoder) throws -> Void)
```

## Parameters 

`custom`  

A closure that receives the data to encode and the encoder instance to encode to.

## Discussion

If the user-defined function throws, the error propagates upward.

If the user-defined function doesn’t perform any encoding at all, the encoder produces an empty JSON object instead.

## See Also

### Custom Formats

case formatted(DateFormatter)

The strategy that defers formatting settings to a supplied date formatter.

