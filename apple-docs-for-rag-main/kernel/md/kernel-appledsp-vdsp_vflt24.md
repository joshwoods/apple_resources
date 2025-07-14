

- Kernel
- AppleDSP
-  vDSP_vflt24 

Function

# vDSP_vflt24

Converts signed 24-bit integer values to single-precision floating-point values.

macOS 10.9+

``` source
void vDSP_vflt24(const vDSP_int24 *vDSP_input1, ptrdiff_t vDSP_stride1, float *vDSP_input2, ptrdiff_t vDSP_stride2, size_t vDSP_size);
```

## Parameters 

`__A`  

The 24-bit integer input vector.

`__IA`  

The stride for input vector `A`.

`__C`  

The single-precision floating-point output vector.

`__IC`  

The stride for output vector `C`.

`__N`  

The number of values to convert.

## Discussion

Converts the signed 24-bit integer values in the input vector `A` to single precision floating-point values and places the results in the output vector `C`.

This function performs the following operation:

    for (n = 0; n &lt; N; ++n)
        C[n*IC] = (float)A[n*IA];

## See Also

### Conversion Functions

vDSP_vsmfix24

Scales and converts single-precision floating-point values to signed 24-bit integer values.

vDSP_vsmfixu24

Scales and converts single-precision floating-point values to unsigned 24-bit integer values.

vDSP_vfix16

Converts an array of single-precision floating-point values to signed 16-bit integer values, rounding toward zero.

vDSP_vfix32

Converts an array of single-precision floating-point values to signed 32-bit integer values, rounding toward zero.

vDSP_vflt16

Converts an array of signed 16-bit integers to single-precision floating-point values.

vDSP_vflt32

Converts an array of signed 32-bit integers to single-precision floating-point values.

vDSP_vfltu24

Converts unsigned 24-bit integer values to single-precision floating-point values.

