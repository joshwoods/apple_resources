

- Accelerate
-  vDSP_DFT_Interleaved_DestroySetupD(\_:) 

Function

# vDSP_DFT_Interleaved_DestroySetupD(\_:)

Releases a double-precision discrete Fourier transform (DFT) setup structure.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func vDSP_DFT_Interleaved_DestroySetupD(_ Setup: vDSP_DFT_Interleaved_SetupD?)
```

## Parameters 

`Setup`  

The setup structure to destroy.

## Discussion

Important

This function isn’t fully thread-safe. Don’t call this function concurrently with any function that uses or shares its underlying storage with the setup structure.

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

func vDSP_DFT_Interleaved_ExecuteD(vDSP_DFT_Interleaved_SetupD, UnsafePointer&lt;DSPDoubleComplex>, UnsafeMutablePointer&lt;DSPDoubleComplex>)

Calculates the double-precision discrete Fourier transform (DFT) for a vector of interleaved complex values.

func vDSP_DFT_Interleaved_DestroySetup(vDSP_DFT_Interleaved_Setup?)

Releases a single-precision discrete Fourier transform (DFT) setup structure.

