

- Accelerate
-  vDSP_DFT_Interleaved_ExecuteD(\_:\_:\_:) 

Function

# vDSP_DFT_Interleaved_ExecuteD(\_:\_:\_:)

Calculates the double-precision discrete Fourier transform (DFT) for a vector of interleaved complex values.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func vDSP_DFT_Interleaved_ExecuteD(
    _ Setup: vDSP_DFT_Interleaved_SetupD,
    _ Iri: UnsafePointer,
    _ Ori: UnsafeMutablePointer
)
```

## Parameters 

`Setup`  

The DFT setup structure for this transform.

`Iri`  

A double-precision vector that contains the input values.

`Ori`  

A double-precision vector that contains the output values. The output can equal the input, but this function doesn’t support any other overlap of the input and output vectors.

## Discussion

This function supports in-place operation where the output and input parameters are equal. The transform length must equal the transform length specified in the setup structure.

Important

For best performance, make sure the two vector addresses you pass to this function are 16-byte-aligned.

## See Also

### Interleaved discrete Fourier transform functions

Performing Fourier transforms on interleaved-complex data

Optimize discrete Fourier transform (DFT) performance with the vDSP interleaved DFT routines.

func vDSP_DFT_Interleaved_CreateSetup(vDSP_DFT_Interleaved_Setup?, vDSP_Length, vDSP_DFT_Direction, vDSP_DFT_RealtoComplex) -> vDSP_DFT_Interleaved_Setup?

Returns a setup structure that contains precalculated data for forward and inverse, single-precision interleaved discrete Fourier transform (DFT) functions.

func vDSP_DFT_Interleaved_CreateSetupD(vDSP_DFT_Interleaved_SetupD?, vDSP_Length, vDSP_DFT_Direction, vDSP_DFT_RealtoComplex) -> vDSP_DFT_Interleaved_SetupD?

Returns a setup structure that contains precalculated data for forward and inverse, double-precision interleaved discrete Fourier transform (DFT) functions.

func vDSP_DFT_Interleaved_Execute(vDSP_DFT_Interleaved_Setup, UnsafePointer&lt;DSPComplex>, UnsafeMutablePointer&lt;DSPComplex>)

Calculates the single-precision discrete Fourier transform (DFT) for a vector of interleaved complex values.

func vDSP_DFT_Interleaved_DestroySetup(vDSP_DFT_Interleaved_Setup?)

Releases a single-precision discrete Fourier transform (DFT) setup structure.

func vDSP_DFT_Interleaved_DestroySetupD(vDSP_DFT_Interleaved_SetupD?)

Releases a double-precision discrete Fourier transform (DFT) setup structure.

