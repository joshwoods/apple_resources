

- Swift
- Array
-  index(\_:offsetBy:) 

Instance Method

# index(\_:offsetBy:)

Returns an index that is the specified distance from the given index.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func index(
    _ i: Int,
    offsetBy distance: Int
) -> Int
```

## Parameters 

`i`  

A valid index of the array.

`distance`  

The distance to offset `i`.

## Return Value

An index offset by `distance` from the index `i`. If `distance` is positive, this is the same value as the result of `distance` calls to `index(after:)`. If `distance` is negative, this is the same value as the result of `abs(distance)` calls to `index(before:)`.

## Discussion

The following example obtains an index advanced four positions from an array’s starting index and then prints the element at that position.

```
let numbers = [10, 20, 30, 40, 50]
let i = numbers.index(numbers.startIndex, offsetBy: 4)
print(numbers[i])
// Prints "50"
```

The value passed as `distance` must not offset `i` beyond the bounds of the collection.

## See Also

### Manipulating Indices

var startIndex: Int

The position of the first element in a nonempty array.

var endIndex: Int

The array’s “past the end” position—that is, the position one greater than the last valid subscript argument.

func index(after: Int) -> Int

Returns the position immediately after the given index.

func formIndex(after: inout Int)

Replaces the given index with its successor.

func index(before: Int) -> Int

Returns the position immediately before the given index.

func formIndex(before: inout Int)

Replaces the given index with its predecessor.

func formIndex(inout Self.Index, offsetBy: Int)

Offsets the given index by the specified distance.

func index(Int, offsetBy: Int, limitedBy: Int) -> Int?

Returns an index that is the specified distance from the given index, unless that distance is beyond a given limiting index.

func formIndex(inout Self.Index, offsetBy: Int, limitedBy: Self.Index) -> Bool

Offsets the given index by the specified distance, or so that it equals the given limiting index.

func distance(from: Int, to: Int) -> Int

Returns the distance between two indices.

