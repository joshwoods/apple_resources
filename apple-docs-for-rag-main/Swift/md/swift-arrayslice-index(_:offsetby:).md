

- Swift
- ArraySlice
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

