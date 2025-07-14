

- Swift
- Float16
-  isEqual(to:) 

Instance Method

# isEqual(to:)

Returns a Boolean value indicating whether this instance is equal to the given value.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
func isEqual(to other: Float16) -> Bool
```

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

