

- Swift
-  min(\_:\_:) 

Function

# min(\_:\_:)

Returns the lesser of two comparable values.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func min(
    _ x: T,
    _ y: T
) -> T where T : Comparable
```

## Parameters 

`x`  

A value to compare.

`y`  

Another value to compare.

## Return Value

The lesser of `x` and `y`. If `x` is equal to `y`, returns `x`.

## See Also

### Choosing the Smallest and Largest Value

func min&lt;T>(T, T, T, T...) -> T

Returns the least argument passed.

func max&lt;T>(T, T) -> T

Returns the greater of two comparable values.

func max&lt;T>(T, T, T, T...) -> T

Returns the greatest argument passed.

