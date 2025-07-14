

- Swift
- Float80
-  isLess(than:) 

Instance Method

# isLess(than:)

Returns a Boolean value indicating whether this instance is less than the given value.

macOS 10.10+

``` source
func isLess(than other: Float80) -> Bool
```

## Parameters 

`other`  

The value to compare with this value.

## Return Value

`true` if this value is less than `other`; otherwise, `false`. If either this value or `other` is NaN, the result of this method is `false`.

## Discussion

This method serves as the basis for the less-than operator (`IEEE 754 specification.

