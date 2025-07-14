

- Accelerate
- vDSP
-  Vector summation 

API Collection

# Vector summation

Sum the values in a vector.

## Topics

### Vector Summation

static func sum&lt;U>(U) -> Double

Returns the double-precision vector sum.

static func sum&lt;U>(U) -> Float

Returns the single-precision vector sum.

static func sumAndSumOfSquares&lt;U>(U) -> (elementsSum: Double, squaresSum: Double)

Returns the double-precision vector sum and sum of squares.

static func sumAndSumOfSquares&lt;U>(U) -> (elementsSum: Float, squaresSum: Float)

Returns the single-precision vector sum and sum of squares.

static func sumOfMagnitudes&lt;U>(U) -> Double

Returns the double-precision vector sum of magnitudes.

static func sumOfMagnitudes&lt;U>(U) -> Float

Returns the single-precision vector sum of magnitudes.

static func sumOfSquares&lt;U>(U) -> Double

Returns the double-precision vector sum of squares.

static func sumOfSquares&lt;U>(U) -> Float

Returns the single-precision vector sum of squares.

vDSP_sve

Calculates the sum of values in a single-precision vector.

vDSP_sveD

Calculates the sum of values in a double-precision vector.

vDSP_svemg

Calculates the sum of magnitudes in a single-precision vector.

vDSP_svemgD

Calculates the sum of magnitudes in a double-precision vector.

vDSP_svesq

Calculates the sum of squares in a single-precision vector.

vDSP_svesqD

Calculates the sum of squares in a double-precision vector.

vDSP_sve_svesq

Calculates the sum of values and the sum of squares in a single-precision vector.

vDSP_sve_svesqD

Calculates the sum of values and the sum of squares in a double-precision vector.

vDSP_svs

Calculates the sum of signed squares in a single-precision vector.

vDSP_svsD

Calculates the sum of signed squares in a double-precision vector.

## See Also

### Vector reduction

Vector extrema calculation

Calculate the minimum and maximum values in a vector.

Vector average calculation

Calculate the average value in a vector.

