

- Accelerate
- vDSP
-  Complex vector conversion 

API Collection

# Complex vector conversion

Perform element-wise split-complex to interleaved and interleaved to split-complex conversion.

## Topics

### Converting interleaved-complex vectors to split-complex vectors

static func convert(interleavedComplexVector: [DSPComplex], toSplitComplexVector: inout DSPSplitComplex)

Converts the contents of an interleaved single-precision complex vector to a split complex vector.

static func convert(interleavedComplexVector: [DSPDoubleComplex], toSplitComplexVector: inout DSPDoubleSplitComplex)

Converts the contents of an interleaved double-precision complex vector to a split complex vector.

vDSP_ctoz

Copies the contents of an interleaved single-precision complex vector to a split complex vector.

vDSP_ctozD

Copies the contents of an interleaved double-precision complex vector to a split complex vector.

### Converting split-complex vectors to interleaved-complex vectors

static func convert(splitComplexVector: DSPSplitComplex, toInterleavedComplexVector: inout [DSPComplex])

Converts the contents of a split single-precision complex vector to an interleaved vector.

static func convert(splitComplexVector: DSPDoubleSplitComplex, toInterleavedComplexVector: inout [DSPDoubleComplex])

Converts the contents of a split double-precision complex vector to an interleaved vector.

vDSP_ztoc

Copies the contents of a split single-precision complex vector to an interleaved vector.

vDSP_ztocD

Copies the contents of a split double-precision complex vector to an interleaved vector.

## See Also

### Vector conversion functions

Conversion to decibel equivalents

Convert vectors that contain power or amplitude data to decibels.

Type conversion

Perform element-wise floating-point to integer and integer to floating-point conversion.

Polar-rectangular conversion

Convert each element of a vector between radius-angle and Cartesian pairs.

