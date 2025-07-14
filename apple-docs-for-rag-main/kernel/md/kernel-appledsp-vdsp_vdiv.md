

- Kernel
- AppleDSP
-  vDSP_vdiv 

Function

# vDSP_vdiv

Divides two single-precision vectors.

macOS 10.4+

``` source
void vDSP_vdiv(const float *__B, vDSP_Stride __IB, const float *__A, vDSP_Stride __IA, float *__C, vDSP_Stride __IC, vDSP_Length __N);
```

## Parameters 

`__B`  

The single-precision real input vector `B`.

`__IB`  

The stride for input vector `B`.

`__A`  

The single-precision real input vector `A`.

`__IA`  

The stride for input vector `A`.

`__C`  

The single-precision real output vector `C`.

`__IC`  

The stride for output vector `C`.

`__N`  

The number of elements to process.

## Discussion

This function calculates the first `N` elements of `A` divided by the corresponding element in `B`, writing the result to `C`:

The operation is:

 for (n = 0; n &lt; N; ++n)
    C[n] = A[n] / B[n];

The following code shows an example of using vDSP_vdiv:

## See Also

### Vector Arithmetic Functions

vDSP_vadd

Adds two single-precision vectors.

vDSP_vma

Adds a single-precision vector to the product of two single-precision vectors.

vDSP_vsub

Subtracts two single-precision vectors.

vDSP_vmul

Multiplies two single-precision vectors.

vDSP_vsmul

Multiplies a single-precision scalar value by a single-precision vector.

