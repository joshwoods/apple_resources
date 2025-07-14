

- Accelerate
- vDSP
-  Vector distance and Pythagorean computation 

API Collection

# Vector distance and Pythagorean computation

Calculate distance and hypotenuse of vectors.

## Topics

### Vector hypotenuse computation

static func hypot&lt;U, V>(U, V) -> [Float]

Returns the single-precision hypotenuses of right triangles with legs that are the lengths of corresponding elements of the two input vectors.

static func hypot&lt;U, V>(U, V) -> [Double]

Returns the double-precision hypotenuses of right triangles with legs that are the lengths of corresponding elements of the two input vectors.

static func hypot&lt;T, U, V>(T, U, result: inout V)

Calculates the single-precision hypotenuses of right triangles with legs that are the lengths of corresponding elements of the two input vectors.

static func hypot&lt;T, U, V>(T, U, result: inout V)

Calculates the double-precision hypotenuses of right triangles with legs that are the lengths of corresponding elements of the two input vectors.

static func hypot&lt;R, S, T, U>(x0: R, x1: S, y0: T, y1: U) -> [Float]

Returns the single-precision hypotenuses of right triangles with legs that are the differences of corresponding elements of two pairs of vectors.

static func hypot&lt;R, S, T, U>(x0: R, x1: S, y0: T, y1: U) -> [Double]

Returns the double-precision hypotenuses of right triangles with legs that are the differences of corresponding elements of two pairs of vectors.

static func hypot&lt;R, S, T, U, V>(x0: R, x1: S, y0: T, y1: U, result: inout V)

Calculates the single-precision hypotenuses of right triangles with legs that are the differences of corresponding elements of two pairs of vectors.

static func hypot&lt;R, S, T, U, V>(x0: R, x1: S, y0: T, y1: U, result: inout V)

Calculates the double-precision hypotenuses of right triangles with legs that are the differences of corresponding elements of two pairs of vectors.

### Vector Pythagorean computation

vDSP_vpythg

Calculates the single-precision hypotenuses of right triangles with legs that are the differences of corresponding elements of two pairs of vectors.

vDSP_vpythgD

Calculates the double-precision hypotenuses of right triangles with legs that are the differences of corresponding elements of two pairs of vectors.

### Vector distance computation

vDSP_vdist

Calculates the single-precision hypotenuses of right triangles with legs that are the lengths of corresponding elements of two pairs of vectors.

vDSP_vdistD

Calculates the double-precision hypotenuses of right triangles with legs that are the lengths of corresponding elements of two pairs of vectors.

static func distanceSquared&lt;U, V>(U, V) -> Float

Returns the single-precision distance squared between two points in n-dimensional space.

static func distanceSquared&lt;U, V>(U, V) -> Double

Returns the double-precision distance squared between two points in n-dimensional space.

vDSP_distancesq

Calculates the single-precision distance squared between two points in n-dimensional space.

vDSP_distancesqD

Calculates the double-precision distance squared between two points in n-dimensional space.

## See Also

### Vector geometry functions

Dot product calculation

Calculate the scalar product of two vectors.

