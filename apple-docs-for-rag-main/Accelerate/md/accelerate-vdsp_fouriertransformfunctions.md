

- Accelerate
-  vDSP_FourierTransformFunctions 

Protocol

# vDSP_FourierTransformFunctions

A protocol that defines functions for fast Fourier transform operations.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
protocol vDSP_FourierTransformFunctions
```

## Topics

### Associated Types

associatedtype SplitComplex

**Required**

### Type Methods

static func destroySetup(OpaquePointer)

**Required**

static func makeFFTSetup(log2n: vDSP_Length, radix: vDSP.Radix) -> OpaquePointer?

**Required**

static func transform(fftSetup: OpaquePointer, log2n: vDSP_Length, source: UnsafePointer&lt;Self.SplitComplex>, destination: UnsafeMutablePointer&lt;Self.SplitComplex>, direction: vDSP.FourierTransformDirection)

**Required**

static func transform2D(fftSetup: OpaquePointer, width: Int, height: Int, source: UnsafePointer&lt;Self.SplitComplex>, destination: UnsafeMutablePointer&lt;Self.SplitComplex>, direction: vDSP.FourierTransformDirection)

**Required**

## Relationships

### Conforming Types

- vDSP_SplitComplexDouble
- vDSP_SplitComplexFloat

## See Also

### Fourier Transform

protocol vDSP_DFTFunctions

A protocol that defines functions for discrete Fourier transform operations.

Deprecated

protocol vDSP_FloatingPointDiscreteFourierTransformable

Types that support discrete Fourier transform operations.

Deprecated

protocol vDSP_FourierTransformable

Types that support fast Fourier transform operations.

protocol vDSP_DiscreteFourierTransformable

protocol vDSP_DiscreteTransformLifecycleFunctions

