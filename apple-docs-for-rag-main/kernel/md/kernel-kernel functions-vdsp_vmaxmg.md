

- Kernel
- Kernel Functions
-  vDSP_vmaxmg 

Function

# vDSP_vmaxmg

Calculates the single-precision maximum magnitude of the corresponding values of two vectors using specified strides.

macOS 10.4+

``` source
void vDSP_vmaxmg(const float *__A, vDSP_Stride __IA, const float *__B, vDSP_Stride __IB, float *__C, vDSP_Stride __IC, vDSP_Length __N);
```

## Parameters 

`__A`  

Single-precision real input vector.

`__IA`  

Stride for `A`.

`__B`  

Single-precision real input vector.

`__IB`  

Stride for `B`.

`__C`  

Single-precision real output vector.

`__IC`  

Stride for `C`.

`__N`  

The number of elements to process

## Discussion

This function compares the magnitudes (absolute values) of the first `N` elements of `A` with corresponding elements of `B`, leaving the greater (or equal) values as corresponding elements of `C`:

for (n = 0; n &lt; N; ++n)
    C[n] = |B[n]| &lt;= |A[n]| ? |A[n]| : |B[n]|;

