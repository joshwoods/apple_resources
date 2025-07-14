

- Foundation
- Measurement
-  ==(\_:\_:) 

Operator

# ==(\_:\_:)

Compare two measurements of the same `Dimension`.

iOS 10.0+iPadOS 10.0+Mac Catalyst 10.0+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
static func == (lhs: Measurement, rhs: Measurement) -> Bool where LeftHandSideType : Unit, RightHandSideType : Unit
```

Available when `UnitType` inherits `Unit`.

## Return Value

`true` if the measurements are equal.

## Discussion

If `lhs.unit == rhs.unit`, returns `lhs.value == rhs.value`. Otherwise, converts `rhs` to the same unit as `lhs` and then compares the resulting values.

## See Also

### Comparing Measurement Attributed Styles

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

