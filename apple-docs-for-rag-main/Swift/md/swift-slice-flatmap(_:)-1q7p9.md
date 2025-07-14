

- Swift
- Slice
-  flatMap(\_:) 

Instance Method

# flatMap(\_:)

Returns the concatenated results of mapping the given transformation over this sequence.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func flatMap(_ transform: @escaping (Self.Elements.Element) -> SegmentOfResult) -> LazySequence>> where SegmentOfResult : Sequence
```

## Discussion

Use this method to receive a single-level sequence when your transformation produces a sequence or collection for each element. Calling `flatMap(_:)` on a sequence `s` is equivalent to calling `s.map(transform).joined()`.

Complexity

O(1)

