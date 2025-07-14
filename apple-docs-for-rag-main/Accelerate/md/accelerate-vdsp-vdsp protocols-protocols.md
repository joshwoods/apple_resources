

- Accelerate
- vDSP
-  vDSP Protocols 

API Collection

# vDSP Protocols

Protocols that support Swift implementations of vDSP operations.

## Topics

### Essentials

protocol AccelerateBuffer

A type that represents an immutable buffer.

protocol AccelerateMutableBuffer

A type that represents a mutable buffer.

protocol AccelerateMatrixBuffer

protocol AccelerateMutableMatrixBuffer

enum AccelerateMatrixOrder

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

protocol vDSP_DiscreteTransformLifecycleFunctions

### Biquadratic Filtering

protocol vDSP_BiquadFunctions

A protocol that defines functions for biquadratic filtering.

protocol vDSP_FloatingPointBiquadFilterable

Types that support biquadratic filtering.

### Type Conversion

protocol vDSP_FloatingPointConvertable

Types that are convertible from integer values.

protocol vDSP_IntegerConvertable

Types that are convertible from floating point values.

### Vector Generation

protocol vDSP_FloatingPointGeneratable

Types that support vectorized window generation.

## See Also

### Swift overlay

enum vDSP

An enumeration that acts as a namespace for Swift overlays to vDSP.

