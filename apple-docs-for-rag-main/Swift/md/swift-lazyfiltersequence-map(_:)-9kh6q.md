

- Swift
- LazyFilterSequence
-  map(\_:) 

Instance Method

# map(\_:)

Returns a `LazyMapSequence` over this `Sequence`. The elements of the result are computed lazily, each time they are read, by calling `transform` function on a base element.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func map(_ transform: @escaping (Self.Element) -> U) -> LazyMapSequence
```

