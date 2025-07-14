

- RealityKit
- Entity
- Entity.ChildCollection
-  indices 

Instance Property

# indices

The indices that are valid for subscripting the collection, in ascending order.

RealityKitSwiftiOSiPadOSMac CatalystmacOSvisionOS

``` source
var indices: DefaultIndices { get }
```

Available when `Indices` is `DefaultIndices`.

## Discussion

A collection’s `indices` property can hold a strong reference to the collection itself, causing the collection to be non-uniquely referenced. If you mutate the collection while iterating over its indices, a strong reference can cause an unexpected copy of the collection. To avoid the unexpected copy, use the `index(after:)` method starting with `startIndex` to produce indices instead.

```
var c = MyFancyCollection([10, 20, 30, 40, 50])
var i = c.startIndex
while i != c.endIndex {
    c[i] /= 5
    i = c.index(after: i)
}
// c == MyFancyCollection([2, 4, 6, 8, 10])
```

## See Also

### Manipulating indices

func distance(from: Self.Index, to: Self.Index) -> Int

Returns the distance between two indices.

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

