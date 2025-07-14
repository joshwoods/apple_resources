

- Foundation
- Measurement
-  -(\_:\_:) 

Operator

# -(\_:\_:)

Subtract two measurements of the same Dimension.

iOS 10.0+iPadOS 10.0+Mac Catalyst 10.0+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
static func - (lhs: Measurement, rhs: Measurement) -> Measurement
```

Available when `UnitType` inherits `Dimension`.

## Return Value

The result of adding the two measurements.

## Discussion

If the `unit` of the `lhs` and `rhs` are `==`, then this returns the result of subtracting the `value` of each `Measurement`. If they are not equal, then this will convert both to the base unit of the `Dimension` and return the result as a `Measurement` of that base unit.

## See Also

### Operating on a Measurement

static func * (Double, Measurement&lt;UnitType>) -> Measurement&lt;UnitType>

Multiply a scalar value by a measurement.

static func * (Measurement&lt;UnitType>, Double) -> Measurement&lt;UnitType>

Multiply a measurement by a scalar value.

static func + (Measurement&lt;UnitType>, Measurement&lt;UnitType>) -> Measurement&lt;UnitType>

Add two measurements.

static func + (Measurement&lt;UnitType>, Measurement&lt;UnitType>) -> Measurement&lt;UnitType>

Adds two measurements of the same dimension.

static func - (Measurement&lt;UnitType>, Measurement&lt;UnitType>) -> Measurement&lt;UnitType>

Subtract two measurements of the same Unit.

static func / (Double, Measurement&lt;UnitType>) -> Measurement&lt;UnitType>

Divide a scalar value by a measurement.

static func / (Measurement&lt;UnitType>, Double) -> Measurement&lt;UnitType>

Divide a measurement by a scalar value.

