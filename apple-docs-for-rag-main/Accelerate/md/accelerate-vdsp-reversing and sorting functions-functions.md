

- Accelerate
- vDSP
-  Reversing and sorting functions 

API Collection

# Reversing and sorting functions

Perform in-place reverse and sort operations on a vector.

## Topics

### Vector reversing functions

static func reverse&lt;V>(inout V)

Reverses a vector of single-precision values in-place.

static func reverse&lt;V>(inout V)

Reverses a vector of double-precision values in-place.

vDSP_vrvrs

Performs an in-place reversal of a single-precision vector.

vDSP_vrvrsD

Performs an in-place reversal of a double-precision vector.

### Vector sorting functions

The functions in this group sort the values in a vector.

static func sort&lt;V>(inout V, sortOrder: vDSP.SortOrder)

Sorts a vector of single-precision values in-place.

static func sort&lt;V>(inout V, sortOrder: vDSP.SortOrder)

Sorts a vector of double-precision values in-place.

enum SortOrder

Constants that specify the sorting order.

vDSP_vsort

Performs an in-place sort of a single-precision vector.

vDSP_vsortD

Performs an in-place sort of a double-precision vector.

vDSP_vsorti

Performs an in-place sort of the indices into a single-precision vector.

vDSP_vsortiD

Performs an in-place sort of the indices into a double-precision vector.

## See Also

### Vector operations

Compression and gathering functions

Compress vectors based on the nonzero elements in a gating vector, or gather vectors based on a separate vector that contains indices.

Copying, element swapping, and merging functions

Copy, swap, and merge the elements of two vectors.

