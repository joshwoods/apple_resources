

- Kernel
- AppleDSP
-  vDSP_vfix16 

Function

# vDSP_vfix16

Converts an array of single-precision floating-point values to signed 16-bit integer values, rounding toward zero.

macOS 10.4+

``` source
void vDSP_vfix16(const float *vDSP_input1, ptrdiff_t vDSP_stride1, int16_t *vDSP_input2, ptrdiff_t vDSP_stride2, size_t vDSP_size);
```

## Parameters 

`__A`  

The single-precision floating-point input vector.

`__IA`  

The stride for input vector `A`.

`__C`  

The 16-bit integer output vector.

`__IC`  

The stride for output vector `C`.

`__N`  

The number of values to convert.

## Discussion

If the resulting value is outside the bounds of the output type, the behavior is undefined. If you need to handle out-of-bounds data, use one of the functions under the “Clipping Operations” topic of Clipping, limit, and threshold operations.

## See Also

### Conversion Functions

vDSP_vsmfix24

Scales and converts single-precision floating-point values to signed 24-bit integer values.

vDSP_vsmfixu24

Scales and converts single-precision floating-point values to unsigned 24-bit integer values.

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

