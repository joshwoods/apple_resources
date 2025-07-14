

- Swift
- Float80
-  addingProduct(\_:\_:) 

Instance Method

# addingProduct(\_:\_:)

Returns the result of adding the product of the two given values to this value, computed without intermediate rounding.

macOS 10.10+

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

