

- Foundation
- Measurement
-  \

Operator

# \

Compare two measurements of the same `Unit`.

iOS 10.0+iPadOS 10.0+Mac Catalyst 10.0+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
static func (lhs: Measurement, rhs: Measurement) -> Bool where LeftHandSideType : Unit, RightHandSideType : Unit
```

Available when `UnitType` inherits `Unit`.

## Return Value

`true` if the measurements can be compared and the `lhs` is less than the `rhs` converted value.

## See Also

### Comparing Measurements

static func > (Self, Self) -> Bool

Returns a Boolean value indicating whether the value of the first argument is greater than that of the second argument.

static func >= (Self, Self) -> Bool

Returns a Boolean value indicating whether the value of the first argument is greater than or equal to that of the second argument.

static func &lt;= (Self, Self) -> Bool

Returns a Boolean value indicating whether the value of the first argument is less than or equal to that of the second argument.

