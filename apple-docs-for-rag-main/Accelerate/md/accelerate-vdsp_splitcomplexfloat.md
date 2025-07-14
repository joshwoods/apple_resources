

- Accelerate
-  vDSP_SplitComplexFloat 

Structure

# vDSP_SplitComplexFloat

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
struct vDSP_SplitComplexFloat
```

## Topics

### Type Methods

static func destroySetup(OpaquePointer)

Releases an FFT setup object.

static func makeFFTSetup(log2n: vDSP_Length, radix: vDSP.Radix) -> OpaquePointer?

Returns a setup structure to perform a fast Fourier transform.

static func transform(fftSetup: OpaquePointer, log2n: vDSP_Length, source: UnsafePointer&lt;vDSP_SplitComplexFloat.SplitComplex>, destination: UnsafeMutablePointer&lt;vDSP_SplitComplexFloat.SplitComplex>, direction: vDSP.FourierTransformDirection)

Performs a 1D fast Fourier transform.

static func transform2D(fftSetup: OpaquePointer, width: Int, height: Int, source: UnsafePointer&lt;vDSP_SplitComplexFloat.SplitComplex>, destination: UnsafeMutablePointer&lt;vDSP_SplitComplexFloat.SplitComplex>, direction: vDSP.FourierTransformDirection)

Performs a 2D fast Fourier transform.

## Relationships

### Conforms To

- vDSP_FourierTransformFunctions

## See Also

### Structures

struct Biquad

A single- or double-precision biquadratic filter.

struct VectorizableDouble

A structure that represents a double-precision real value for biquadratic filtering and discrete Fourier transforms.

struct VectorizableFloat

A structure that represents a single-precision real value for biquadratic filtering and discrete Fourier transforms.

struct DFTDoublePrecisionInterleavedFunctions

struct DFTDoublePrecisionSplitComplexFunctions

struct DFTSinglePrecisionInterleavedFunctions

struct DFTSinglePrecisionSplitComplexFunctions

struct vDSP_SplitComplexDouble

