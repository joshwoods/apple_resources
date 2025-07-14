

- Swift
- Int32
-  words 

Instance Property

# words

A collection containing the words of this value’s binary representation, in order from the least significant to most significant.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var words: Int32.Words { get }
```

## Discussion

Negative values are returned in two’s complement representation, regardless of the type’s underlying implementation.

