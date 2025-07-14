

- Kernel
- Kernel Functions
-  vLL128Shift 

Function

# vLL128Shift

128-bit logical left shift.

macOS 10.5+

``` source
vUInt32 vLL128Shift(vUInt32 vA, vUInt8 vShiftFactor);
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

