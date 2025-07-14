

- Swift
- Collection
-  index(after:) 

Instance Method

# index(after:)

Returns the position immediately after the given index.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func index(after i: Self.Index) -> Self.Index
```

**Required** Default implementation provided.

## Parameters 

`i`  

A valid index of the collection. `i` must be less than `endIndex`.

## Return Value

The index value immediately after `i`.

## Discussion

The successor of an index must be well defined. For an index `i` into a collection `c`, calling `c.index(after: i)` returns the same index every time.

## Default Implementations

### BidirectionalCollection Implementations

func index(after: Self.Index) -> Self.Index

Returns the position immediately after the given index.

## See Also

### Manipulating Indices

var startIndex: Self.Index

The position of the first element in a nonempty collection.

**Required**

var endIndex: Self.Index

The collection’s “past the end” position—that is, the position one greater than the last valid subscript argument.

**Required**

var indices: Self.Indices

The indices that are valid for subscripting the collection, in ascending order.

**Required** Default implementations provided.

func formIndex(inout Self.Index, offsetBy: Int)

Offsets the given index by the specified distance.

func formIndex(inout Self.Index, offsetBy: Int, limitedBy: Self.Index) -> Bool

Offsets the given index by the specified distance, or so that it equals the given limiting index.

