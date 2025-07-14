

- Swift
- String
-  index(\_:offsetBy:) 

Instance Method

# index(\_:offsetBy:)

Returns an index that is the specified distance from the given index.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func index(
    _ i: String.Index,
    offsetBy distance: Int
) -> String.Index
```

## Parameters 

`i`  

A valid index of the collection.

`distance`  

The distance to offset `i`.

## Return Value

An index offset by `distance` from the index `i`. If `distance` is positive, this is the same value as the result of `distance` calls to `index(after:)`. If `distance` is negative, this is the same value as the result of `abs(distance)` calls to `index(before:)`.

## Discussion

The following example obtains an index advanced four positions from a string’s starting index and then prints the character at that position.

```
let s = "Swift"
let i = s.index(s.startIndex, offsetBy: 4)
print(s[i])
// Prints "t"
```

The value passed as `distance` must not offset `i` beyond the bounds of the collection.

Complexity

O(*n*), where *n* is the absolute value of `distance`.

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

func index(String.Index, offsetBy: Int, limitedBy: String.Index) -> String.Index?

Returns an index that is the specified distance from the given index, unless that distance is beyond a given limiting index.

func formIndex(inout Self.Index, offsetBy: Int)

Offsets the given index by the specified distance.

func formIndex(inout Self.Index, offsetBy: Int, limitedBy: Self.Index) -> Bool

Offsets the given index by the specified distance, or so that it equals the given limiting index.

func distance(from: String.Index, to: String.Index) -> Int

Returns the distance between two indices.

var indices: DefaultIndices&lt;Self>

The indices that are valid for subscripting the collection, in ascending order.

