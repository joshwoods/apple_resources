

- Kernel
- AppleDSP
-  vDSP_vsmfixu24 

Function

# vDSP_vsmfixu24

Scales and converts single-precision floating-point values to unsigned 24-bit integer values.

macOS 10.9+

``` source
void vDSP_vsmfixu24(const float vDSP_input1[], ptrdiff_t vDSP_stride1, const float vDSP_input2[], vDSP_uint24 *vDSP_input3, ptrdiff_t vDSP_stride2, size_t vDSP_size);
```

## Parameters 

`__A`  

The single-precision floating-point input vector.

`__IA`  

The stride for input vector `A`.

`__B`  

A pointer to a floating-point scaling factor.

`__C`  

The 24-bit integer output vector.

`__IC`  

The stride for output vector `C`.

`__N`  

The number of values to convert.

## Discussion

This function scales vector `A` by the scalar `*B` and converts each resulting value to an unsigned 24-bit integer, placing the results in `C`. After scaling, the function clamps values that are outside the range that unsigned 24-bit integers can represent to the largest or smallest representable values.

This function performs the following operations:

In this pseudocode, `UINT24_MAX` is equal to `2^24 - 1`.

## See Also

### Conversion Functions

vDSP_vsmfix24

Scales and converts single-precision floating-point values to signed 24-bit integer values.

vDSP_vfix16

Converts an array of single-precision floating-point values to signed 16-bit integer values, rounding toward zero.

vDSP_vfix32

Converts an array of single-precision floating-point values to signed 32-bit integer values, rounding toward zero.

vDSP_vflt16

Converts an array of signed 16-bit integers to single-precision floating-point values.

vDSP_vflt24

Converts signed 24-bit integer values to single-precision floating-point values.

vDSP_vflt32

Converts an array of signed 32-bit integers to single-precision floating-point values.

vDSP_vfltu24

Converts unsigned 24-bit integer values to single-precision floating-point values.

