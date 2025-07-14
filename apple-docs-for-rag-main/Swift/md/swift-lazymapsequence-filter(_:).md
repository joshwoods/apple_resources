

- Swift
- LazyMapSequence
-  filter(\_:) 

Instance Method

# filter(\_:)

Returns the elements of `self` that satisfy `isIncluded`.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func filter(_ isIncluded: @escaping (Self.Elements.Element) -> Bool) -> LazyFilterSequence
```

## Discussion

Note

The elements of the result are computed on-demand, as the result is used. No buffering storage is allocated and each traversal step invokes `predicate` on one or more underlying elements.

