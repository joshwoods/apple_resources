

- Swift
- FloatingPoint
-  isLessThanOrEqualTo(\_:) 

Instance Method

# isLessThanOrEqualTo(\_:)

Returns a Boolean value indicating whether this instance is less than or equal to the given value.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func isLessThanOrEqualTo(_ other: Self) -> Bool
```

**Required**

## Parameters 

`other`  

The value to compare with this value.

## Return Value

`true` if `other` is greater than this value; otherwise, `false`. If either this value or `other` is NaN, the result of this method is `false`.

## Discussion

This method serves as the basis for the less-than-or-equal-to operator (`IEEE 754 specification.

