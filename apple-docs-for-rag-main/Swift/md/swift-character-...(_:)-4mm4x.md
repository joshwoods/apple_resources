

- Swift
- Character
-  ...(\_:) 

Operator

# ...(\_:)

Returns a partial range up to, and including, its upper bound.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static func ... (maximum: Self) -> PartialRangeThrough
```

## Parameters 

`maximum`  

The upper bound for the range.

## Discussion

Use the prefix closed range operator (prefix `...`) to create a partial range of any type that conforms to the `Comparable` protocol. This example creates a `PartialRangeThrough` instance that includes any value less than or equal to `5.0`.

```
let throughFive = ...5.0

throughFive.contains(4.0)     // true
throughFive.contains(5.0)     // true
throughFive.contains(6.0)     // false
```

You can use this type of partial range of a collection’s indices to represent the range from the start of the collection up to, and including, the partial range’s upper bound.

```
let numbers = [10, 20, 30, 40, 50, 60, 70]
print(numbers[...3])
// Prints "[10, 20, 30, 40]"
```

Precondition

`maximum` must compare equal to itself (i.e. cannot be NaN).

## See Also

### Creating a Range Expression

static func ... (Self, Self) -> ClosedRange&lt;Self>

Returns a closed range that contains both of its bounds.

static func ... (Self) -> PartialRangeFrom&lt;Self>

Returns a partial range extending upward from a lower bound.

