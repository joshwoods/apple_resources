

- Kernel
- Kernel Functions
-  vDSP_zmmul 

Function

# vDSP_zmmul

Multiplies two matrices of single-precision complex numbers out-of-place.

macOS 10.2+

``` source
void vDSP_zmmul(const DSPSplitComplex *__A, vDSP_Stride __IA, const DSPSplitComplex *__B, vDSP_Stride __IB, const DSPSplitComplex *__C, vDSP_Stride __IC, vDSP_Length __M, vDSP_Length __N, vDSP_Length __P);
```

## Parameters 

`__A`  

Single-precision complex `M`-by-`P` input matrix.

`__IA`  

Stride for `A`.

`__B`  

Single-precision complex `P`-by-`N`input matrix.

`__IB`  

Stride for `B`.

`__C`  

Single-precision complex `M`-by-`N` result matrix.

`__IC`  

Stride for `C`.

`__M`  

The number of rows in matrices `A` and `C`.

`__N`  

The number of columns in matrices `B` and `C`.

`__P`  

The number of columns in matrix `A` and the number of rows in matrix `B`.

## Discussion

This function performs an out-of-place complex multiplication of an `M`-by-`P` matrix `A` by a `P`-by-`N` matrix `B` and stores the results in an `M`-by-`N` matrix `C`.

This performs the following operation:

