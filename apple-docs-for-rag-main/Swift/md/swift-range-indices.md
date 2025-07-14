

- Swift
- Range
-  indices 

Instance Property

# indices

The indices that are valid for subscripting the range, in ascending order.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var indices: Range.Indices { get }
```

Available when `Bound` conforms to `Strideable` and `Bound.Stride` conforms to `SignedInteger`.

