

- Swift
- PartialRangeFrom
-  makeIterator() 

Instance Method

# makeIterator()

Returns an iterator for this sequence.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func makeIterator() -> PartialRangeFrom.Iterator
```

Available when `Bound` conforms to `Strideable` and `Bound.Stride` conforms to `SignedInteger`.

