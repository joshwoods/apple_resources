

- Swift
- ClosedRange
-  ==(\_:\_:) 

Operator

# ==(\_:\_:)

Returns a Boolean value indicating whether two ranges are equal.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static func == (lhs: ClosedRange, rhs: ClosedRange) -> Bool
```

Available when `Bound` conforms to `Comparable`.

## Parameters 

`lhs`  

A range to compare.

`rhs`  

Another range to compare.

## Discussion

Two ranges are equal when they have the same lower and upper bounds.

```
let x = 5...15
print(x == 5...15)
// Prints "true"
print(x == 10...20)
// Prints "false"
```

## See Also

### Comparing Ranges

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

func overlaps(Range&lt;Bound>) -> Bool

Returns a Boolean value indicating whether this range and the given range contain an element in common.

func overlaps(ClosedRange&lt;Bound>) -> Bool

Returns a Boolean value indicating whether this range and the given closed range contain an element in common.

