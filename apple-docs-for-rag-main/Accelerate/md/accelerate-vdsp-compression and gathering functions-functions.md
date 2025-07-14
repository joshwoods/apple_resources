

- Accelerate
- vDSP
-  Compression and gathering functions 

API Collection

# Compression and gathering functions

Compress vectors based on the nonzero elements in a gating vector, or gather vectors based on a separate vector that contains indices.

## Topics

### Vector compression

The functions in this group compress an input vector by eliminating elements that correspond to zero values in a gating vector.

static func compress&lt;T, U>(T, gatingVector: U, nonZeroGatingCount: Int?) -> [Float]

Returns a compressed copy of the specified single-precision vector using the nonzero values in a gating vector.

static func compress&lt;T, U>(T, gatingVector: U, nonZeroGatingCount: Int?) -> [Double]

Returns a compressed copy of the specified double-precision vector using the nonzero values in a gating vector.

static func compress&lt;T, U, V>(T, gatingVector: U, result: inout V)

Compresses the specified single-precision vector using the nonzero values in a gating vector.

static func compress&lt;T, U, V>(T, gatingVector: U, result: inout V)

Compresses the specified double-precision vector using the nonzero values in a gating vector.

vDSP_vcmprs

Generates a compressed copy of the specified single-precision vector using the nonzero values in a gating vector.

vDSP_vcmprsD

Generates a compressed copy of the specified double-precision vector using the nonzero values in a gating vector.

### Vector gathering functions

The functions in this group use indices or pointers stored in a source vector to generate a new vector with elements from a second source vector or memory.

static func gather&lt;T, U>(T, indices: U) -> [Float]

Returns a gathered copy of the specified single-precision vector using a vector that defines the indices to keep.

static func gather&lt;T, U>(T, indices: U) -> [Double]

Returns a gathered copy of the specified double-precision vector using a vector that defines the indices to keep.

static func gather&lt;T, U, V>(T, indices: U, result: inout V)

Gathers the specified single-precision vector using a vector that defines the indices to keep.

static func gather&lt;T, U, V>(T, indices: U, result: inout V)

Gathers the specified double-precision vector using a vector that defines the indices to keep.

vDSP_vindex

Generates a gathered copy of the specified single-precision vector using a vector that defines the zero-based indices to keep.

vDSP_vindexD

Generates a gathered copy of the specified double-precision vector using a vector that defines the zero-based indices to keep.

vDSP_vgathr

Generates a gathered copy of the specified single-precision vector using a vector that defines the one-based indices to keep.

vDSP_vgathrD

Generates a gathered copy of the specified double-precision vector using a vector that defines the one-based indices to keep.

vDSP_vgathra

Generates a gathered copy of the specified single-precision vector using a vector that defines the pointers to the values to keep.

vDSP_vgathraD

Generates a gathered copy of the specified double-precision vector using a vector that defines the pointers to the values to keep.

## See Also

### Vector operations

Copying, element swapping, and merging functions

Copy, swap, and merge the elements of two vectors.

Reversing and sorting functions

Perform in-place reverse and sort operations on a vector.

