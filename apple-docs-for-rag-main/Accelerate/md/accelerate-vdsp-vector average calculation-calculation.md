

- Accelerate
- vDSP
-  Vector average calculation 

API Collection

# Vector average calculation

Calculate the average value in a vector.

## Topics

### Calculating the mean value of a vector

static func mean&lt;U>(U) -> Float

Returns the mean value of a single-precision vector.

static func mean&lt;U>(U) -> Double

Returns the mean value of a double-precision vector.

vDSP_meanv

Calculates the mean value of a single-precision vector.

vDSP_meanvD

Calculates the mean value of a double-precision vector.

### Calculating the mean of magnitudes of a vector

static func meanMagnitude&lt;U>(U) -> Float

Returns the mean of magnitudes of a single-precision vector.

static func meanMagnitude&lt;U>(U) -> Double

Returns the mean of magnitudes of a double-precision vector.

vDSP_meamgv

Calculates the mean of magnitudes of a single-precision vector.

vDSP_meamgvD

Calculates the mean of magnitudes of a double-precision vector.

### Calculating the mean of squares of a vector

static func meanSquare&lt;U>(U) -> Float

Returns the mean of squares of a single-precision vector.

static func meanSquare&lt;U>(U) -> Double

Returns the mean of squares of a double-precision vector.

vDSP_measqv

Calculates the mean of squares of a single-precision vector.

vDSP_measqvD

Calculates the mean of squares of a double-precision vector.

vDSP_mvessq

Calculates the mean of signed squares of a single-precision vector.

vDSP_mvessqD

Calculates the mean of signed squares of a double-precision vector.

### Calculating the root mean square of a vector

static func rootMeanSquare&lt;U>(U) -> Float

Returns the root mean square of a single-precision vector.

static func rootMeanSquare&lt;U>(U) -> Double

Returns the root mean square of a double-precision vector.

vDSP_rmsqv

Calculates the root mean square of a single-precision vector.

vDSP_rmsqvD

Calculates the root mean square of a double-precision vector.

## See Also

### Vector reduction

Vector extrema calculation

Calculate the minimum and maximum values in a vector.

Vector summation

Sum the values in a vector.

