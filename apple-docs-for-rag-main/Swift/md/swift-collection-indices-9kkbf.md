

- Swift
- Collection
-  indices 

Instance Property

# indices

The indices that are valid for subscripting the collection, in ascending order.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var indices: Self.Indices { get }
```

**Required** Default implementations provided.

## Discussion

A collection’s `indices` property can hold a strong reference to the collection itself, causing the collection to be nonuniquely referenced. If you mutate the collection while iterating over its indices, a strong reference can result in an unexpected copy of the collection. To avoid the unexpected copy, use the `index(after:)` method starting with `startIndex` to produce indices instead.

```
var c = MyFancyCollection([10, 20, 30, 40, 50])
var i = c.startIndex
while i != c.endIndex {
    c[i] /= 5
    i = c.index(after: i)
}
// c == MyFancyCollection([2, 4, 6, 8, 10])
```

## Default Implementations

### BidirectionalCollection Implementations

var indices: Range&lt;Self.Index>

The indices that are valid for subscripting the collection, in ascending order.

### Collection Implementations

var indices: DefaultIndices&lt;Self>

The indices that are valid for subscripting the collection, in ascending order.

## See Also

### Manipulating Indices

var startIndex: Self.Index

The position of the first element in a nonempty collection.

**Required**

var endIndex: Self.Index

The collection’s “past the end” position—that is, the position one greater than the last valid subscript argument.

**Required**

func index(after: Self.Index) -> Self.Index

Returns the position immediately after the given index.

**Required** Default implementation provided.

func formIndex(inout Self.Index, offsetBy: Int)

Offsets the given index by the specified distance.

func formIndex(inout Self.Index, offsetBy: Int, limitedBy: Self.Index) -> Bool

Offsets the given index by the specified distance, or so that it equals the given limiting index.

