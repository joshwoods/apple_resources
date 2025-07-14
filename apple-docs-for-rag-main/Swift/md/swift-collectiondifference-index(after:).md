

- Swift
- CollectionDifference
-  index(after:) 

Instance Method

# index(after:)

Returns the position immediately after the given index.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func index(after index: CollectionDifference.Index) -> CollectionDifference.Index
```

## Return Value

The index value immediately after `i`.

## Discussion

The successor of an index must be well defined. For an index `i` into a collection `c`, calling `c.index(after: i)` returns the same index every time.

