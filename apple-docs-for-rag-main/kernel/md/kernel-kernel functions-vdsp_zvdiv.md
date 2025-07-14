

- Kernel
- Kernel Functions
-  vDSP_zvdiv 

Function

# vDSP_zvdiv

Complex vector_vector divide; single precision.

macOS 10.4+

``` source
void vDSP_zvdiv(const DSPSplitComplex *__B, vDSP_Stride __IB, const DSPSplitComplex *__A, vDSP_Stride __IA, const DSPSplitComplex *__C, vDSP_Stride __IC, vDSP_Length __N);
```

## Parameters 

`__B`  

Single-precision complex input vector. Note that `B` comes before `A`!

`__IB`  

Stride for `B`.

`__A`  

Single-precision complex input vector.

`__IA`  

Stride for `A`.

`__C`  

Single-precision complex output vector.

`__IC`  

Stride for `C`.

`__N`  

The number of elements to process.

## Discussion

This function divides the first `N` elements of `A` by corresponding elements of `B`, leaving the result in `C`.

