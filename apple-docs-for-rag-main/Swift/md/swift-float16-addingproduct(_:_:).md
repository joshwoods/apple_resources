

- Swift
- Float16
-  addingProduct(\_:\_:) 

Instance Method

# addingProduct(\_:\_:)

Returns the result of adding the product of the two given values to this value, computed without intermediate rounding.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func addingProduct(
    _ lhs: Self,
    _ rhs: Self
) -> Self
```

## Parameters 

`lhs`  

One of the values to multiply before adding to this value.

`rhs`  

The other value to multiply.

## Return Value

The product of `lhs` and `rhs`, added to this value.

## Discussion

This method is equivalent to the C `fma` function and implements the `fusedMultiplyAdd` operation defined by the IEEE 754 specification.

