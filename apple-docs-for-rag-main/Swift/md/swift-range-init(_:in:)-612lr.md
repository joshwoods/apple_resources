

- Swift
- Range
-  init(\_:in:) 

Initializer

# init(\_:in:)

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
init?(
    _ region: R,
    in attributedString: S
) where R : RangeExpression, S : AttributedStringProtocol, R.Bound == String.Index
```

Available when `Bound` is `AttributedString.Index`.

