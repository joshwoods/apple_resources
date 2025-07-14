

- Kernel
- Kernel Functions
-  vDSP_zvmov 

Function

# vDSP_zvmov

Complex vector copy; single precision.

macOS 10.4+

``` source
void vDSP_zvmov(const DSPSplitComplex *__A, vDSP_Stride __IA, const DSPSplitComplex *__C, vDSP_Stride __IC, vDSP_Length __N);
```

## Parameters 

`__A`  

Single-precision complex input vector.

`__IA`  

Address stride for `A`.

`__C`  

Single-precision complex output vector.

`__IC`  

Address stride for `C`.

`__N`  

The number of elements to process.

## Discussion

Copies complex vector `A` to complex vector `C`.

