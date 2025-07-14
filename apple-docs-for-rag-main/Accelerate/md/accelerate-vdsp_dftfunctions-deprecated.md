

- Accelerate
-  vDSP_DFTFunctions Deprecated

Protocol

# vDSP_DFTFunctions

A protocol that defines functions for discrete Fourier transform operations.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
protocol vDSP_DFTFunctions
```

Deprecated

Use `vDSP.DiscreteFourierTransform`.

## Topics

### Associated Types

associatedtype Scalar

**Required**

### Type Methods

static func destroySetup(OpaquePointer)

**Required**

static func makeDFTSetup&lt;T>(previous: vDSP.DFT&lt;T>?, count: Int, direction: vDSP.FourierTransformDirection, transformType: vDSP.DFTTransformType) -> OpaquePointer?

**Required**

static func transform&lt;U, V>(dftSetup: OpaquePointer, inputReal: U, inputImaginary: U, outputReal: inout V, outputImaginary: inout V)

**Required**

## Relationships

### Conforming Types

- vDSP.VectorizableDouble
- vDSP.VectorizableFloat

## See Also

### Fourier Transform

protocol vDSP_FloatingPointDiscreteFourierTransformable

Types that support discrete Fourier transform operations.

Deprecated

protocol vDSP_FourierTransformFunctions

A protocol that defines functions for fast Fourier transform operations.

protocol vDSP_FourierTransformable

Types that support fast Fourier transform operations.

protocol vDSP_DiscreteFourierTransformable

protocol vDSP_DiscreteTransformLifecycleFunctions

