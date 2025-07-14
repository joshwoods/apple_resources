

- Accelerate
- vDSP
-  Vector clear and fill functions 

API Collection

# Vector clear and fill functions

Populate vectors with zeros or a scalar value.

## Topics

### Clearing Vectors

static func clear&lt;V>(inout V)

Populates a double-precision vector with zeros.

static func clear&lt;V>(inout V)

Populates a single-precision vector with zeros.

vDSP_vclr

Populates a single-precision vector with zeros.

vDSP_vclrD

Populates a double-precision vector with zeros.

### Filling Vectors with a Single Scalar Value

static func fill&lt;V>(inout V, with: Double)

Populates a double-precision vector with a specified scalar value.

static func fill&lt;V>(inout V, with: Float)

Populates a single-precision vector with a specified scalar value.

vDSP_vfill

Populates a single-precision vector with a specified scalar value.

vDSP_vfillD

Populates a double-precision vector with a specified scalar value.

vDSP_vfilli

Populates an integer vector with a specified scalar value.

vDSP_zvfill

Populates a complex single-precision vector with a specified scalar value.

vDSP_zvfillD

Populates a complex double-precision vector with a specified scalar value.

## See Also

### Vector generation, filling, and clearing

Vector generation

Populate vectors with ramps, values from lookup tables, interpolated values, and window functions.

