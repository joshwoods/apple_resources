

- Accelerate
-  vDSP_DiscreteTransformLifecycleFunctions 

Protocol

# vDSP_DiscreteTransformLifecycleFunctions

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOSwatchOS 8.0+

``` source
protocol vDSP_DiscreteTransformLifecycleFunctions
```

## Topics

### Type Methods

static func destroySetup(OpaquePointer)

**Required**

static func makeDiscreteFourierTransform(previous: OpaquePointer?, count: Int, direction: vDSP.FourierTransformDirection, transformType: vDSP.DFTTransformType) throws -> OpaquePointer

**Required**

## Relationships

### Conforming Types

- vDSP.DFTDoublePrecisionInterleavedFunctions
- vDSP.DFTDoublePrecisionSplitComplexFunctions
- vDSP.DFTSinglePrecisionInterleavedFunctions
- vDSP.DFTSinglePrecisionSplitComplexFunctions

## See Also

### Fourier Transform

protocol vDSP_DFTFunctions

A protocol that defines functions for discrete Fourier transform operations.

Deprecated

protocol vDSP_FloatingPointDiscreteFourierTransformable

Types that support discrete Fourier transform operations.

Deprecated

protocol vDSP_FourierTransformFunctions

A protocol that defines functions for fast Fourier transform operations.

protocol vDSP_FourierTransformable

Types that support fast Fourier transform operations.

protocol vDSP_DiscreteFourierTransformable

