

- Create ML Components
- AnnotatedFiles
-  index(after:) 

Instance Method

# index(after:)

Returns the position immediately after the given index.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
func index(after i: AnnotatedFiles.Index) -> AnnotatedFiles.Index
```

## Parameters 

`i`  

A valid index of the collection. `i` must be less than `endIndex`.

## Return Value

The index value immediately after `i`.

## Discussion

The successor of an index must be well defined. For an index `i` into a collection `c`, calling `c.index(after: i)` returns the same index every time.

## See Also

### Getting the index

typealias Index

A type that represents a position in the collection.

typealias Element

A type representing the sequence’s elements.

