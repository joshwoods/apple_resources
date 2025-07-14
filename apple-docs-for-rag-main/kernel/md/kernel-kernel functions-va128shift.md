

- Kernel
- Kernel Functions
-  vA128Shift 

Function

# vA128Shift

128-bit arithmetic (signed) shift.

macOS 10.0+

``` source
vUInt32 vA128Shift(vUInt32 vA, vUInt8 vShiftFactor);
```

## Parameters 

`vA`  

The vector to shift.

`vShiftFactor`  

The number of bits to shift the vector.

## Return Value

Returns the shifted vector.

## Discussion

This function treats the entire 128-bit vector as a single value to shift.

