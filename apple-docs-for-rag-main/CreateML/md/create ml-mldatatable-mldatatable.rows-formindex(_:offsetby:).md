

- Create ML
- MLDataTable
- MLDataTable.Rows
-  formIndex(\_:offsetBy:) 

Instance Method

# formIndex(\_:offsetBy:)

Offsets the given index by the specified distance.

Create MLSwiftiOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+tvOS 16.0+visionOS 1.0+

``` source
func formIndex(
    _ i: inout Self.Index,
    offsetBy distance: Int
)
```

## Parameters 

`i`  

A valid index of the collection.

`distance`  

The distance to offset `i`. `distance` must not be negative unless the collection conforms to the `BidirectionalCollection` protocol.

## Discussion

The value passed as `distance` must not offset `i` beyond the bounds of the collection.

Complexity

O(1) if the collection conforms to `RandomAccessCollection`; otherwise, O(*k*), where *k* is the absolute value of `distance`.

## See Also

### Manipulating indices

var startIndex: Int

The position of the first row in a nonempty DataTable. If the DataTable is empty, `startIndex` is equal to `endIndex`.

var endIndex: Int

The DataTable’s “past the end” position—that is, the position one greater than the last valid subscript argument.

func formIndex(after: inout Self.Index)

Replaces the given index with its successor.

func formIndex(before: inout Self.Index)

Replaces the given index with its predecessor.

func index(Self.Index, offsetBy: Int, limitedBy: Self.Index) -> Self.Index?

Returns an index that is the specified distance from the given index, unless that distance is beyond a given limiting index.

func formIndex(inout Self.Index, offsetBy: Int, limitedBy: Self.Index) -> Bool

Offsets the given index by the specified distance, or so that it equals the given limiting index.

