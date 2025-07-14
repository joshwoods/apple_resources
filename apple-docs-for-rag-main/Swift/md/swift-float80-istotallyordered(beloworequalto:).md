

- Swift
- Float80
-  isTotallyOrdered(belowOrEqualTo:) 

Instance Method

# isTotallyOrdered(belowOrEqualTo:)

Returns a Boolean value indicating whether this instance should precede or tie positions with the given value in an ascending sort.

macOS 10.10+

``` source
func isTotallyOrdered(belowOrEqualTo other: Self) -> Bool
```

## Parameters 

`other`  

A floating-point value to compare to this value.

## Return Value

`true` if this value is ordered below or the same as `other` in a total ordering of the floating-point type; otherwise, `false`.

## Discussion

This relation is a refinement of the less-than-or-equal-to operator (`

```
var numbers = [2.5, 21.25, 3.0, .nan, -9.5]
numbers.sort { !$1.isTotallyOrdered(belowOrEqualTo: $0) }
print(numbers)
// Prints "[-9.5, 2.5, 3.0, 21.25, nan]"
```

The `isTotallyOrdered(belowOrEqualTo:)` method implements the total order relation as defined by the IEEE 754 specification.

