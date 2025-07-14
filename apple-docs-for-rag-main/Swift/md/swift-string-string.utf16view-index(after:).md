

- Swift
- String
- String.UTF16View
-  index(after:) 

Instance Method

# index(after:)

Returns the position immediately after the given index.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func index(after idx: String.UTF16View.Index) -> String.UTF16View.Index
```

## Return Value

The index value immediately after `i`.

## Discussion

The successor of an index must be well defined. For an index `i` into a collection `c`, calling `c.index(after: i)` returns the same index every time.

