

- Swift
- Float16
-  isLessThanOrEqualTo(\_:) 

Instance Method

# isLessThanOrEqualTo(\_:)

Returns a Boolean value indicating whether this instance is less than or equal to the given value.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
func isLessThanOrEqualTo(_ other: Float16) -> Bool
```

## Parameters 

`other`  

The value to compare with this value.

## Return Value

`true` if `other` is greater than this value; otherwise, `false`. If either this value or `other` is NaN, the result of this method is `false`.

## Discussion

This method serves as the basis for the less-than-or-equal-to operator (`IEEE 754 specification.

