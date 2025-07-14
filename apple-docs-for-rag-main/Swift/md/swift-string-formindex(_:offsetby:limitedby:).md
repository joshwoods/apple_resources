

- Swift
- String
-  formIndex(\_:offsetBy:limitedBy:) 

Instance Method

# formIndex(\_:offsetBy:limitedBy:)

Offsets the given index by the specified distance, or so that it equals the given limiting index.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func formIndex(
    _ i: inout Self.Index,
    offsetBy distance: Int,
    limitedBy limit: Self.Index
) -> Bool
```

## Parameters 

`i`  

A valid index of the collection.

`distance`  

The distance to offset `i`. `distance` must not be negative unless the collection conforms to the `BidirectionalCollection` protocol.

`limit`  

A valid index of the collection to use as a limit. If `distance > 0`, a limit that is less than `i` has no effect. Likewise, if `distance 

## Return Value

`true` if `i` has been offset by exactly `distance` steps without going beyond `limit`; otherwise, `false`. When the return value is `false`, the value of `i` is equal to `limit`.

## Discussion

The value passed as `distance` must not offset `i` beyond the bounds of the collection, unless the index passed as `limit` prevents offsetting beyond those bounds.

Complexity

O(1) if the collection conforms to `RandomAccessCollection`; otherwise, O(*k*), where *k* is the absolute value of `distance`.

## See Also

### Manipulating Indices

var startIndex: String.Index

The position of the first character in a nonempty string.

var endIndex: String.Index

A string’s “past the end” position—that is, the position one greater than the last valid subscript argument.

func index(after: String.Index) -> String.Index

Returns the position immediately after the given index.

func formIndex(after: inout Self.Index)

Replaces the given index with its successor.

func index(before: String.Index) -> String.Index

Returns the position immediately before the given index.

func formIndex(before: inout Self.Index)

Replaces the given index with its predecessor.

func index(String.Index, offsetBy: Int) -> String.Index

Returns an index that is the specified distance from the given index.

func index(String.Index, offsetBy: Int, limitedBy: String.Index) -> String.Index?

Returns an index that is the specified distance from the given index, unless that distance is beyond a given limiting index.

func formIndex(inout Self.Index, offsetBy: Int)

Offsets the given index by the specified distance.

func distance(from: String.Index, to: String.Index) -> Int

Returns the distance between two indices.

var indices: DefaultIndices&lt;Self>

The indices that are valid for subscripting the collection, in ascending order.

