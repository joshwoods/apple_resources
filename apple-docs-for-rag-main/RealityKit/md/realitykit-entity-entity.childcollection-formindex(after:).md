

- RealityKit
- Entity
- Entity.ChildCollection
-  formIndex(after:) 

Instance Method

# formIndex(after:)

Replaces the given index with its successor.

RealityKitSwiftiOSiPadOSMac CatalystmacOSvisionOS

``` source
func formIndex(after i: inout Self.Index)
```

## Parameters 

`i`  

A valid index of the collection. `i` must be less than `endIndex`.

## See Also

### Manipulating indices

func distance(from: Self.Index, to: Self.Index) -> Int

Returns the distance between two indices.

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

func index(Self.Index, offsetBy: Int) -> Self.Index

Returns an index that is the specified distance from the given index.

func index(Self.Index, offsetBy: Int, limitedBy: Self.Index) -> Self.Index?

Returns an index that is the specified distance from the given index, unless that distance is beyond a given limiting index.

func index(after: Int) -> Int

Returns the position immediately after the given index. (See `Collection.index`.)

func index(of: Self.Element) -> Self.Index?

Returns the first index where the specified value appears in the collection.

