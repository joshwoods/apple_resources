

- Accelerate
- vDSP
-  vDSP.DFTSinglePrecisionSplitComplexFunctions 

Structure

# vDSP.DFTSinglePrecisionSplitComplexFunctions

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOSwatchOS 8.0+

``` source
struct DFTSinglePrecisionSplitComplexFunctions
```

## Topics

### Type Methods

static func destroySetup(OpaquePointer)

static func makeDiscreteFourierTransform(previous: OpaquePointer?, count: Int, direction: vDSP.FourierTransformDirection, transformType: vDSP.DFTTransformType) throws -> OpaquePointer

## Relationships

### Conforms To

- vDSP_DiscreteTransformLifecycleFunctions

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

struct vDSP_SplitComplexDouble

struct vDSP_SplitComplexFloat

