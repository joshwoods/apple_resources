

- Accelerate
-  DSPSplitComplex 

Structure

# DSPSplitComplex

A structure that represents a single-precision complex vector with the real and imaginary parts stored in separate arrays.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct DSPSplitComplex
```

## Mentioned in 

Finding the component frequencies in a composite sine wave

Controlling vDSP operations with stride

Performing Fourier Transforms on Multiple Signals

Performing Fourier transforms on interleaved-complex data

## Topics

### Creating a Split Complex Structure

init(realp: UnsafeMutablePointer&lt;Float>, imagp: UnsafeMutablePointer&lt;Float>)

Creates a new split complex structure.

### Inspecting a Split Complex Structure’s Data

var imagp: UnsafeMutablePointer&lt;Float>

An array of imaginary parts of the complex numbers.

var realp: UnsafeMutablePointer&lt;Float>

An array of real parts of the complex numbers.

### Initializers

init(fromInputArray: [Float], realParts: inout [Float], imaginaryParts: inout [Float])Deprecated

## Relationships

### Conforms To

- BitwiseCopyable
- Copyable
- vDSP_FourierTransformable

## See Also

### Data types

typealias vDSP_Length

An unsigned-integer value that represents the size of vectors and the indices of elements in vectors.

typealias vDSP_Stride

An integer value that represents the differences between indices of elements, including the lengths of strides.

struct DSPComplex

A structure that represents a single-precision complex value.

typealias COMPLEX_SPLIT

struct DSPDoubleComplex

A structure that represents a double-precision complex value.

typealias DOUBLE_COMPLEX_SPLIT

struct DSPDoubleSplitComplex

A structure that represents a double-precision complex vector with the real and imaginary parts stored in separate arrays.

struct VectorizableDouble

A structure that represents a double-precision real value for biquadratic filtering and discrete Fourier transforms.

struct VectorizableFloat

A structure that represents a single-precision real value for biquadratic filtering and discrete Fourier transforms.

