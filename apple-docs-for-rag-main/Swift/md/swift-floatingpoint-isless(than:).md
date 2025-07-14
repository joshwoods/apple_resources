

- Swift
- FloatingPoint
-  isLess(than:) 

Instance Method

# isLess(than:)

Returns a Boolean value indicating whether this instance is less than the given value.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func isLess(than other: Self) -> Bool
```

**Required**

## Parameters 

`other`  

The value to compare with this value.

## Return Value

`true` if this value is less than `other`; otherwise, `false`. If either this value or `other` is NaN, the result of this method is `false`.

## Discussion

This method serves as the basis for the less-than operator (`IEEE 754 specification.

