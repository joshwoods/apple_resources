

- Kernel
- Kernel Functions
-  vDSP_zvabs 

Function

# vDSP_zvabs

Complex vector absolute values; single precision.

macOS 10.4+

``` source
void vDSP_zvabs(const DSPSplitComplex *__A, vDSP_Stride __IA, float *__C, vDSP_Stride __IC, vDSP_Length __N);
```

## Parameters 

`__A`  

Single-precision complex input vector.

`__IA`  

Address stride for `A`.

`__C`  

Single-precision real output vector.

`__IC`  

Address stride for `C`.

`__N`  

The number of elements to process.

## Discussion

This performs the following operation:

