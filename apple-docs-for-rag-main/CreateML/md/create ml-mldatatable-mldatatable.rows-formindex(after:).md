

- Create ML
- MLDataTable
- MLDataTable.Rows
-  formIndex(after:) 

Instance Method

# formIndex(after:)

Replaces the given index with its successor.

Create MLSwiftiOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+tvOS 16.0+visionOS 1.0+

``` source
func formIndex(after i: inout Self.Index)
```

## Parameters 

`i`  

A valid index of the collection. `i` must be less than `endIndex`.

## See Also

### Manipulating indices

var startIndex: Int

The position of the first row in a nonempty DataTable. If the DataTable is empty, `startIndex` is equal to `endIndex`.

var endIndex: Int

The DataTable’s “past the end” position—that is, the position one greater than the last valid subscript argument.

func formIndex(before: inout Self.Index)

Replaces the given index with its predecessor.

func formIndex(inout Self.Index, offsetBy: Int)

Offsets the given index by the specified distance.

func index(Self.Index, offsetBy: Int, limitedBy: Self.Index) -> Self.Index?

Returns an index that is the specified distance from the given index, unless that distance is beyond a given limiting index.

func formIndex(inout Self.Index, offsetBy: Int, limitedBy: Self.Index) -> Bool

Offsets the given index by the specified distance, or so that it equals the given limiting index.

