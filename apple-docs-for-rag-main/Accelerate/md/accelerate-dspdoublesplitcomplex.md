

- Accelerate
-  DSPDoubleSplitComplex 

Structure

# DSPDoubleSplitComplex

A structure that represents a double-precision complex vector with the real and imaginary parts stored in separate arrays.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct DSPDoubleSplitComplex
```

## Topics

### Creating a Split Complex Structure

init(realp: UnsafeMutablePointer&lt;Double>, imagp: UnsafeMutablePointer&lt;Double>)

Creates a new split complex structure.

### Inspecting a Split Complex Structure’s Data

var imagp: UnsafeMutablePointer&lt;Double>

An array of imaginary parts of the complex numbers.

var realp: UnsafeMutablePointer&lt;Double>

An array of real parts of the complex numbers.

### Initializers

init(fromInputArray: [Double], realParts: inout [Double], imaginaryParts: inout [Double])Deprecated

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

struct DSPSplitComplex

A structure that represents a single-precision complex vector with the real and imaginary parts stored in separate arrays.

struct VectorizableDouble

A structure that represents a double-precision real value for biquadratic filtering and discrete Fourier transforms.

struct VectorizableFloat

A structure that represents a single-precision real value for biquadratic filtering and discrete Fourier transforms.

