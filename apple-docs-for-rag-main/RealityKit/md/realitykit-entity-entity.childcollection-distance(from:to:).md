

- RealityKit
- Entity
- Entity.ChildCollection
-  distance(from:to:) 

Instance Method

# distance(from:to:)

Returns the distance between two indices.

RealityKitSwiftiOSiPadOSMac CatalystmacOSvisionOS

``` source
func distance(
    from start: Self.Index,
    to end: Self.Index
) -> Int
```

## Parameters 

`start`  

A valid index of the collection.

`end`  

Another valid index of the collection. If `end` is equal to `start`, the result is zero.

## Return Value

The distance between `start` and `end`. The result can be negative only if the collection conforms to the `BidirectionalCollection` protocol.

## Discussion

Unless the collection conforms to the `BidirectionalCollection` protocol, `start` must be less than or equal to `end`.

Complexity

O(1) if the collection conforms to `RandomAccessCollection`; otherwise, O(*k*), where *k* is the resulting distance.

## See Also

### Manipulating indices

var indices: DefaultIndices&lt;Self>

The indices that are valid for subscripting the collection, in ascending order.

var startIndex: Int

The position of the first element in a nonempty collection. (See `Collection.startIndex`.)

var endIndex: Int

TThe collection’s “past the end” position—that is, the position one greater than the last valid subscript argument. (See `Collection.endIndex`.)

func firstIndex(of: Self.Element) -> Self.Index?

Returns the first index where the specified value appears in the collection.

func firstIndex(where: (Self.Element) throws -> Bool) rethrows -> Self.Index?

Returns the first index in which an element of the collection satisfies the given predicate.

func formIndex(inout Self.Index, offsetBy: Int)

Offsets the given index by the specified distance.

func formIndex(inout Self.Index, offsetBy: Int, limitedBy: Self.Index) -> Bool

Offsets the given index by the specified distance, or so that it equals the given limiting index.

func formIndex(after: inout Self.Index)

Replaces the given index with its successor.

func index(Self.Index, offsetBy: Int) -> Self.Index

Returns an index that is the specified distance from the given index.

func index(Self.Index, offsetBy: Int, limitedBy: Self.Index) -> Self.Index?

Returns an index that is the specified distance from the given index, unless that distance is beyond a given limiting index.

func index(after: Int) -> Int

Returns the position immediately after the given index. (See `Collection.index`.)

func index(of: Self.Element) -> Self.Index?

Returns the first index where the specified value appears in the collection.

