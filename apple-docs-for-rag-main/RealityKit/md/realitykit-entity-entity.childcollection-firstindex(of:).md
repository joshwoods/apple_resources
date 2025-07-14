

- RealityKit
- Entity
- Entity.ChildCollection
-  firstIndex(of:) 

Instance Method

# firstIndex(of:)

Returns the first index where the specified value appears in the collection.

RealityKitSwiftiOSiPadOSMac CatalystmacOSvisionOS

``` source
func firstIndex(of element: Self.Element) -> Self.Index?
```

Available when `Element` conforms to `Equatable`.

## Parameters 

`element`  

An element to search for in the collection.

## Return Value

The first index where `element` is found. If `element` is not found in the collection, returns `nil`.

## Discussion

After using `firstIndex(of:)` to find the position of a particular element in a collection, you can use it to access the element by subscripting. This example shows how you can modify one of the names in an array of students.

```
var students = ["Ben", "Ivy", "Jordell", "Maxime"]
if let i = students.firstIndex(of: "Maxime") {
    students[i] = "Max"
}
print(students)
// Prints "["Ben", "Ivy", "Jordell", "Max"]"
```

Complexity

O(*n*), where *n* is the length of the collection.

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

