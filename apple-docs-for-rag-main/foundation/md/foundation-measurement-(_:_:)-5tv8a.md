

- Foundation
- Measurement
-  \*(\_:\_:) 

Operator

# \*(\_:\_:)

Multiply a measurement by a scalar value.

iOS 10.0+iPadOS 10.0+Mac Catalyst 10.0+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
static func * (lhs: Measurement, rhs: Double) -> Measurement
```

Available when `UnitType` inherits `Unit`.

## Parameters 

`lhs`  

A measurement to multiply.

`rhs`  

A double-precision floating-point number to multiply.

## Return Value

A measurement of value `lhs.value * rhs` with the same unit as `lhs`.

## See Also

### Operating on a Measurement

static func * (Double, Measurement&lt;UnitType>) -> Measurement&lt;UnitType>

Multiply a scalar value by a measurement.

static func + (Measurement&lt;UnitType>, Measurement&lt;UnitType>) -> Measurement&lt;UnitType>

Add two measurements.

static func + (Measurement&lt;UnitType>, Measurement&lt;UnitType>) -> Measurement&lt;UnitType>

Adds two measurements of the same dimension.

static func - (Measurement&lt;UnitType>, Measurement&lt;UnitType>) -> Measurement&lt;UnitType>

Subtract two measurements of the same Unit.

static func - (Measurement&lt;UnitType>, Measurement&lt;UnitType>) -> Measurement&lt;UnitType>

Subtract two measurements of the same Dimension.

static func / (Double, Measurement&lt;UnitType>) -> Measurement&lt;UnitType>

Divide a scalar value by a measurement.

static func / (Measurement&lt;UnitType>, Double) -> Measurement&lt;UnitType>

Divide a measurement by a scalar value.

