

- Swift
-  max(\_:\_:\_:\_:) 

Function

# max(\_:\_:\_:\_:)

Returns the greatest argument passed.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func max(
    _ x: T,
    _ y: T,
    _ z: T,
    _ rest: T...
) -> T where T : Comparable
```

## Parameters 

`x`  

A value to compare.

`y`  

Another value to compare.

`z`  

A third value to compare.

`rest`  

Zero or more additional values.

## Return Value

The greatest of all the arguments. If there are multiple equal greatest arguments, the result is the last one.

## See Also

### Choosing the Smallest and Largest Value

func min&lt;T>(T, T) -> T

Returns the lesser of two comparable values.

func min&lt;T>(T, T, T, T...) -> T

Returns the least argument passed.

func max&lt;T>(T, T) -> T

Returns the greater of two comparable values.

