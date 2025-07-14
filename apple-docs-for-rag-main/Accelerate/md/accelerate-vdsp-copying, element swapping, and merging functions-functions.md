

- Accelerate
- vDSP
-  Copying, element swapping, and merging functions 

API Collection

# Copying, element swapping, and merging functions

Copy, swap, and merge the elements of two vectors.

## Topics

### Vector copying functions

The functions in this group copy one vector to another vector.

static func copy(DSPSplitComplex, to: inout DSPSplitComplex, count: Int)

Copies a complex single-precision vector.

static func copy(DSPDoubleSplitComplex, to: inout DSPDoubleSplitComplex, count: Int)

Copies a complex double-precision vector.

vDSP_zvmov

Moves a complex single-precision vector.

vDSP_zvmovD

Moves a complex double-precision vector.

### Vector-to-vector element swapping functions

static func swapElements&lt;T, U>(inout T, inout U)

Swaps the elements of two single-precision vectors.

static func swapElements&lt;T, U>(inout T, inout U)

Swaps the elements of two double-precision vectors.

vDSP_vswap

Swaps the elements of two single-precision vectors using the specified stride.

vDSP_vswapD

Swaps the elements of two double-precision vectors using the specified stride.

### Vector-to-vector merging functions

static func taperedMerge&lt;T, U>(T, U) -> [Float]

Returns the result of a tapered merge between two single-precision vectors.

static func taperedMerge&lt;T, U>(T, U) -> [Double]

Returns the result of a tapered merge between two double-precision vectors.

static func taperedMerge&lt;T, U, V>(T, U, result: inout V)

Computes the result of a tapered merge between two single-precision vectors.

static func taperedMerge&lt;T, U, V>(T, U, result: inout V)

Computes the result of a tapered merge between two double-precision vectors.

vDSP_vtmerg

Performs a tapered merge between two single-precision vectors.

vDSP_vtmergD

Performs a tapered merge between two double-precision vectors.

## See Also

### Vector operations

Compression and gathering functions

Compress vectors based on the nonzero elements in a gating vector, or gather vectors based on a separate vector that contains indices.

Reversing and sorting functions

Perform in-place reverse and sort operations on a vector.

