

- Kernel
- Kernel Functions
-  vDSP_ctoz 

Function

# vDSP_ctoz

Copies the contents of an interleaved complex vector `C` to a split complex vector `Z`; single precision.

macOS 10.0+

``` source
void vDSP_ctoz(const DSPComplex *__C, vDSP_Stride __IC, const DSPSplitComplex *__Z, vDSP_Stride __IZ, vDSP_Length __N);
```

## Parameters 

`__C`  

Single-precision interleaved complex input vector.

`__IC`  

Stride for `C`; must be an even number.

`__Z`  

Single-precision split-complex output vector.

`__IZ`  

Stride for `Z`.

`__N`  

The number of elements to process.

## Discussion

For best performance, `C`, `Z.realp`, and `Z.imagp` should be 16-byte aligned.

This function performs the following operations:

for (n = 0; n &lt; N; ++n)
{
  Z->realp[n*IZ] = C[n*IC/2].real;
  Z->imagp[n*IZ] = C[n*IC/2].imag;
}

See also functionsvDSP_ztoc and vDSP_ztocD.

