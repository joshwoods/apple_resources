

- Swift
- FloatingPoint
-  isEqual(to:) 

Instance Method

# isEqual(to:)

Returns a Boolean value indicating whether this instance is equal to the given value.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func isEqual(to other: Self) -> Bool
```

**Required**

## Parameters 

`other`  

The value to compare with this value.

## Return Value

`true` if `other` has the same value as this instance; otherwise, `false`. If either this value or `other` is NaN, the result of this method is `false`.

## Discussion

This method serves as the basis for the equal-to operator (`==`) for floating-point values. When comparing two values with this method, `-0` is equal to `+0`. NaN is not equal to any value, including itself. For example:

```
let x = 15.0
x.isEqual(to: 15.0)
// true
x.isEqual(to: .nan)
// false
Double.nan.isEqual(to: .nan)
// false
```

The `isEqual(to:)` method implements the equality predicate defined by the IEEE 754 specification.

