

- Swift
- String
-  distance(from:to:) 

Instance Method

# distance(from:to:)

Returns the distance between two indices.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func distance(
    from start: String.Index,
    to end: String.Index
) -> Int
```

## Parameters 

`start`  

A valid index of the collection.

`end`  

Another valid index of the collection. If `end` is equal to `start`, the result is zero.

## Return Value

The distance between `start` and `end`.

## Discussion

Complexity

O(*n*), where *n* is the resulting distance.

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

func formIndex(inout Self.Index, offsetBy: Int, limitedBy: Self.Index) -> Bool

Offsets the given index by the specified distance, or so that it equals the given limiting index.

var indices: DefaultIndices&lt;Self>

The indices that are valid for subscripting the collection, in ascending order.

