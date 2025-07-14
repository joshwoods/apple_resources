

- TabularData
- Order
-  areOrdered(\_:\_:) 

Instance Method

# areOrdered(\_:\_:)

Returns a Boolean that indicates whether the comparable types match the order’s state.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func areOrdered(
    _ lhs: T,
    _ rhs: T
) -> Bool where T : Comparable
```

## Parameters 

`lhs`  

A comparable type.

`rhs`  

Another comparable type.

## See Also

### Getting the Properties

case ascending

A sort ordering that starts with the lowest value and monotonically proceeds to higher values.

case descending

A sort ordering that starts with the highest value and monotonically proceeds to lower values.

