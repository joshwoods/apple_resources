

- Accelerate
- vDSP
-  Vector extrema calculation 

API Collection

# Vector extrema calculation

Calculate the minimum and maximum values in a vector.

## Topics

### Calculating the minimum value of a vector

static func minimum&lt;U>(U) -> Float

Returns the single-precision minimum value of a vector.

static func minimum&lt;U>(U) -> Double

Returns the double-precision minimum value of a vector.

vDSP_minv

Calculates the single-precision minimum value of a vector.

vDSP_minvD

Calculates the double-precision minimum value of a vector.

vDSP_minmgv

Calculates the single-precision minimum magnitude of a vector.

vDSP_minmgvD

Calculates the double-precision minimum magnitude of a vector.

### Calculating the index of the minimum value of a vector

static func indexOfMinimum&lt;U>(U) -> (UInt, Float)

Returns the maximum value and corresponding index in a single-precision vector.

static func indexOfMinimum&lt;U>(U) -> (UInt, Double)

Returns the maximum value and corresponding index in a double-precision vector.

vDSP_minvi

Calculates the minimum value and corresponding index in a single-precision vector.

vDSP_minviD

Calculates the minimum value and corresponding index in a double-precision vector.

vDSP_minmgvi

Calculates the minimum magnitude and corresponding index in a single-precision vector.

vDSP_minmgviD

Calculates the minimum magnitude and corresponding index in a double-precision vector.

### Calculating the maximum value of a vector

static func maximum&lt;U>(U) -> Float

Returns the single-precision maximum value of a vector.

static func maximum&lt;U>(U) -> Double

Returns the double-precision maximum value of a vector.

vDSP_maxv

Calculates the single-precision maximum value of a vector.

vDSP_maxvD

Calculates the double-precision maximum value of a vector.

static func maximumMagnitude&lt;U>(U) -> Float

Returns the single-precision maximum magnitude of a vector.

static func maximumMagnitude&lt;U>(U) -> Double

Returns the double-precision maximum magnitude of a vector.

vDSP_maxmgv

Calculates the single-precision maximum magnitude of a vector.

vDSP_maxmgvD

Calculates the double-precision maximum magnitude of a vector.

### Calculating the index of the maximum value of a vector

static func indexOfMaximum&lt;U>(U) -> (UInt, Float)

Returns the maximum value and corresponding index in a single-precision vector.

static func indexOfMaximum&lt;U>(U) -> (UInt, Double)

Returns the maximum value and corresponding index in a double-precision vector.

vDSP_maxvi

Calculates the maximum value and corresponding index in a single-precision vector.

vDSP_maxviD

Calculates the maximum value and corresponding index in a double-precision vector.

static func indexOfMaximumMagnitude&lt;U>(U) -> (UInt, Float)

Returns the maximum magnitude and corresponding index in a single-precision vector.

static func indexOfMaximumMagnitude&lt;U>(U) -> (UInt, Double)

Returns the maximum magnitude and corresponding index in a double-precision vector.

vDSP_maxmgvi

Calculates the maximum magnitude and corresponding index in a single-precision vector.

vDSP_maxmgviD

Calculates the maximum magnitude and corresponding index in a double-precision vector.

## See Also

### Vector reduction

Vector average calculation

Calculate the average value in a vector.

Vector summation

Sum the values in a vector.

