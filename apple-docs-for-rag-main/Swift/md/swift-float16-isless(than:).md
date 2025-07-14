

- Swift
- Float16
-  isLess(than:) 

Instance Method

# isLess(than:)

Returns a Boolean value indicating whether this instance is less than the given value.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
func isLess(than other: Float16) -> Bool
```

## Parameters 

`other`  

The value to compare with this value.

## Return Value

`true` if this value is less than `other`; otherwise, `false`. If either this value or `other` is NaN, the result of this method is `false`.

## Discussion

This method serves as the basis for the less-than operator (`IEEE 754 specification.

