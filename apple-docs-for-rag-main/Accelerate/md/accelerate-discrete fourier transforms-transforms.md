

- Accelerate
-  Discrete Fourier transforms 

API Collection

# Discrete Fourier transforms

Transform vectors of temporal and spatial domain complex values to the frequency domain, and vice versa.

## Topics

### Objects that simplify discrete Fourier transforms

class DiscreteFourierTransform

An object that provides forward and inverse discrete Fourier transforms on single- or double-precision collections of interleaved or split-complex data.

enum DFTTransformType

Discrete Fourier transform types.

class DFT

A single- and double-precision discrete Fourier transform.

Deprecated

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

func vDSP_DFT_Interleaved_DestroySetupD(vDSP_DFT_Interleaved_SetupD?)

Releases a double-precision discrete Fourier transform (DFT) setup structure.

### Real discrete Fourier transform setup

vDSP_DFT_zrop_CreateSetup

Returns a setup structure that contains precalculated data for forward and inverse, real, single-precision DFT functions.

vDSP_DFT_zrop_CreateSetupD

Returns a setup structure that contains precalculated data for forward and inverse, real, double-precision DFT functions.

### Complex discrete Fourier transform setup

vDSP_DFT_zop_CreateSetup

Returns a setup structure that contains precalculated data for forward and inverse, complex, single-precision DFT functions.

vDSP_DFT_zop_CreateSetupD

Returns a setup structure that contains precalculated data for forward and inverse, complex, double-precision DFT functions.

### Functions to perform discrete Fourier transforms

vDSP_DFT_Execute

Calculates the discrete single-precision Fourier transform for a vector.

vDSP_DFT_ExecuteD

Calculates the discrete double-precision Fourier transform for a vector.

### Discrete Fourier transform cleanup

vDSP_DFT_DestroySetup

Releases a single-precision setup structure.

vDSP_DFT_DestroySetupD

Releases a double-precision setup structure.

### Data types

typealias vDSP_DFT_Interleaved_Setup

An opaque type that contains setup information for an interleaved single-precision discrete Fourier transform (DFT).

typealias vDSP_DFT_Interleaved_SetupD

An opaque type that contains setup information for an interleaved double-precision discrete Fourier transform (DFT).

typealias vDSP_DFT_Setup

An opaque type that contains setup information for a single-precision discrete Fourier transform (DFT).

typealias vDSP_DFT_SetupD

An opaque type that contains setup information for a double-precision discrete Fourier transform (DFT).

### Constants

enum vDSP_DFT_Direction

An enumeration that specifies whether to perform a forward or inverse DFT.

### Enumerations

enum vDSP_DFT_RealtoComplex

## See Also

### Fourier and Cosine Transforms

Understanding data packing for Fourier transforms

Format source data for the vDSP Fourier functions, and interpret the results.

Finding the component frequencies in a composite sine wave

Use 1D fast Fourier transform to compute the frequency components of a signal.

Performing Fourier transforms on interleaved-complex data

Optimize discrete Fourier transform (DFT) performance with the vDSP interleaved DFT routines.

Reducing spectral leakage with windowing

Multiply signal data by window sequence values when performing transforms with noninteger period signals.

Signal extraction from noise

Use Accelerate’s discrete cosine transform to remove noise from a signal.

Performing Fourier Transforms on Multiple Signals

Use Accelerate’s multiple-signal fast Fourier transform (FFT) functions to transform multiple signals with a single function call.

Halftone descreening with 2D fast Fourier transform

Reduce or remove periodic artifacts from images.

Fast Fourier transforms

Transform vectors and matrices of temporal and spatial domain complex values to the frequency domain, and vice versa.

Discrete Cosine transforms

Transform vectors of temporal and spatial domain real values to the frequency domain, and vice versa.

