

- Accelerate
- vDSP
-  Polar-rectangular conversion 

API Collection

# Polar-rectangular conversion

Convert each element of a vector between radius-angle and Cartesian pairs.

## Topics

### Converting polar coordinates to rectangular coordinates

static func polarToRectangular&lt;U>(U) -> [Float]

Returns single-precision rectangular coordinates converted from polar coordinates.

static func polarToRectangular&lt;U>(U) -> [Double]

Returns double-precision rectangular coordinates converted from polar coordinates.

static func convert&lt;U, V>(polarCoordinates: U, toRectangularCoordinates: inout V)

Converts single-precision polar coordinates to rectangular coordinates.

static func convert&lt;U, V>(polarCoordinates: U, toRectangularCoordinates: inout V)

Converts double-precision polar coordinates to rectangular coordinates.

vDSP_rect

Converts single-precision polar coordinates to rectangular coordinates, using the specified stride.

vDSP_rectD

Converts double-precision polar coordinates to rectangular coordinates, using the specified stride.

### Converting rectangular coordinates to polar coordinates

static func rectangularToPolar&lt;U>(U) -> [Float]

Returns single-precision polar coordinates converted from rectangular coordinates.

static func rectangularToPolar&lt;U>(U) -> [Double]

Returns double-precision polar coordinates converted from rectangular coordinates.

static func convert&lt;U, V>(rectangularCoordinates: U, toPolarCoordinates: inout V)

Converts single-precision rectangular coordinates to polar coordinates.

static func convert&lt;U, V>(rectangularCoordinates: U, toPolarCoordinates: inout V)

Converts double-precision rectangular coordinates to polar coordinates.

vDSP_polar

Converts single-precision rectangular coordinates to polar coordinates, using the specified stride.

vDSP_polarD

Converts double-precision rectangular coordinates to polar coordinates, using the specified stride.

## See Also

### Vector conversion functions

Conversion to decibel equivalents

Convert vectors that contain power or amplitude data to decibels.

Type conversion

Perform element-wise floating-point to integer and integer to floating-point conversion.

Complex vector conversion

Perform element-wise split-complex to interleaved and interleaved to split-complex conversion.

