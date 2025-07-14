

- Swift
- Range
-  init(\_:in:) 

Initializer

# init(\_:in:)

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
init?(
    _ range: NSRange,
    in string: S
) where S : StringProtocol
```

Available when `Bound` is `String.Index`.

## See Also

### Converting Ranges

func relative&lt;C>(to: C) -> Range&lt;Bound>

Returns the range of indices described by this range expression within the given collection.

init?(NSRange, in: String)

