

- Kernel
- Kernel Functions
-  vDSP_ztoc 

Function

# vDSP_ztoc

Copies the contents of a split complex vector `Z` to an interleaved complex vector `C`; single precision.

macOS 10.0+

``` source
void vDSP_ztoc(const DSPSplitComplex *__Z, vDSP_Stride __IZ, DSPComplex *__C, vDSP_Stride __IC, vDSP_Length __N);
```

## Parameters 

`__Z`  

Single-precision split-complex input vector.

`__IZ`  

Stride for `Z`.

`__C`  

Single-precision interleaved complex output vector.

`__IC`  

Stride for `C`. Must be an even number.

`__N`  

The number of elements to process.

## Discussion

For best performance, `C`, `Z.realp`, and `Z.imagp` should be 16-byte aligned.

This performs the following operations:

for (n = 0; n &lt; N; ++n)
{
  C[n*IC/2].real = Z->realp[n*IZ];
  C[n*IC/2].imag = Z->imagp[n*IZ];
}

See also vDSP_ctoz and vDSP_ctozD.

