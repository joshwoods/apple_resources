

- Accelerate
-  vLR128Shift(\_:\_:) 

Function

# vLR128Shift(\_:\_:)

128-bit logical right shift.

macOS 10.5+

``` source
func vLR128Shift(
    _ vA: vUInt32,
    _ vShiftFactor: vUInt8
) -> vUInt32
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

## See Also

### Shift and Rotate Functions (from vBasicOps.h)

func vLL128Shift(vUInt32, vUInt8) -> vUInt32

128-bit logical left shift.

func vLL64Shift(vUInt32, vUInt8) -> vUInt32

64-bit logical left shift.

func vLL64Shift2(vUInt32, vUInt8) -> vUInt32

64-bit logical left shift with two shift factors.

func vLR64Shift(vUInt32, vUInt8) -> vUInt32

64-bit logical right shift.

func vLR64Shift2(vUInt32, vUInt8) -> vUInt32

64-bit logical right shift with two shift factors.

func vA64Shift(vUInt32, vUInt8) -> vUInt32

64-bit arithmetic (signed) shift.

func vA64Shift2(vUInt32, vUInt8) -> vUInt32

64-bit arithmetic (signed) shift with two shift factors.

func vA128Shift(vUInt32, vUInt8) -> vUInt32

128-bit arithmetic (signed) shift.

func vL64Rotate(vUInt32, vUInt8) -> vUInt32

64-bit left rotate.

func vR64Rotate(vUInt32, vUInt8) -> vUInt32

64-bit right rotate.

func vL64Rotate2(vUInt32, vUInt8) -> vUInt32

64-bit left rotate with two rotation factors.

func vR64Rotate2(vUInt32, vUInt8) -> vUInt32

64-bit right rotate with two rotation factors.

func vL128Rotate(vUInt32, vUInt8) -> vUInt32

128-bit left rotate.

func vR128Rotate(vUInt32, vUInt8) -> vUInt32

128-bit right rotate.

