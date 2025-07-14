

- Accelerate
- vDSP
-  Linear interpolation functions 

API Collection

# Linear interpolation functions

Compute the linear average between two vectors or between the neighboring elements in one vector.

## Topics

### Vector-to-Vector Linear Interpolation

static func linearInterpolate&lt;T, U>(T, U, using: Double) -> [Double]

Returns the linear interpolation between the supplied double-precision vectors.

static func linearInterpolate&lt;T, U>(T, U, using: Float) -> [Float]

Returns the linear interpolation between the supplied single-precision vectors.

static func linearInterpolate&lt;T, U, V>(T, U, using: Double, result: inout V)

Calculates the linear interpolation between the supplied double-precision vectors.

static func linearInterpolate&lt;T, U, V>(T, U, using: Float, result: inout V)

Calculates the linear interpolation between the supplied single-precision vectors.

vDSP_vintb

Calculates the linear interpolation between the supplied single-precision vectors using the specified stride.

vDSP_vintbD

Calculates the linear interpolation between the supplied double-precision vectors using the specified stride.

### Single-Vector Linear Interpolation

The functions in this group calculate the linear interpolation between neighboring elements.

Using linear interpolation to construct new data points

Fill the gaps in arrays of numerical data using linear interpolation.

static func linearInterpolate&lt;T, U>(elementsOf: T, using: U) -> [Double]

Returns the interpolation between the neighboring elements of a double-precision vector.

static func linearInterpolate&lt;T, U>(elementsOf: T, using: U) -> [Float]

Returns the interpolation between the neighboring elements of a single-precision vector.

static func linearInterpolate&lt;T, U, V>(elementsOf: T, using: U, result: inout V)

Calculates the interpolation between the neighboring elements of a double-precision vector.

static func linearInterpolate&lt;T, U, V>(elementsOf: T, using: U, result: inout V)

Calculates the interpolation between the neighboring elements of a single-precision vector.

vDSP_vlint

Calculates the interpolation between the neighboring elements of a single-precision vector using the specified stride.

vDSP_vlintD

Calculates the interpolation between the neighboring elements of a double-precision vector using the specified stride.

## See Also

### Vector interpolation

Quadratic interpolation functions

Compute the quadratic interpolation between the neighboring elements in a vector.

