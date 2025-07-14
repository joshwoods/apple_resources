

- Create ML
- MLDataTable
- MLDataTable.Rows
-  index(\_:offsetBy:limitedBy:) 

Instance Method

# index(\_:offsetBy:limitedBy:)

Returns an index that is the specified distance from the given index, unless that distance is beyond a given limiting index.

Create MLSwiftiOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+tvOS 16.0+visionOS 1.0+

``` source
func index(
    _ i: Self.Index,
    offsetBy distance: Int,
    limitedBy limit: Self.Index
) -> Self.Index?
```

## Parameters 

`i`  

A valid index of the array.

`distance`  

The distance to offset `i`.

`limit`  

A valid index of the collection to use as a limit. If `distance > 0`, `limit` should be greater than `i` to have any effect. Likewise, if `distance 

## Return Value

An index offset by `distance` from the index `i`, unless that index would be beyond `limit` in the direction of movement. In that case, the method returns `nil`.

## Discussion

The following example obtains an index advanced four positions from an array’s starting index and then prints the element at that position. The operation doesn’t require going beyond the limiting `numbers.endIndex` value, so it succeeds.

```
let numbers = [10, 20, 30, 40, 50]
let i = numbers.index(numbers.startIndex, offsetBy: 4)
print(numbers[i])
// Prints "50"
```

The next example attempts to retrieve an index ten positions from `numbers.startIndex`, but fails, because that distance is beyond the index passed as `limit`.

```
let j = numbers.index(numbers.startIndex,
                      offsetBy: 10,
                      limitedBy: numbers.endIndex)
print(j)
// Prints "nil"
```

The value passed as `distance` must not offset `i` beyond the bounds of the collection, unless the index passed as `limit` prevents offsetting beyond those bounds.

Complexity

O(1)

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

func formIndex(inout Self.Index, offsetBy: Int)

Offsets the given index by the specified distance.

func formIndex(inout Self.Index, offsetBy: Int, limitedBy: Self.Index) -> Bool

Offsets the given index by the specified distance, or so that it equals the given limiting index.

