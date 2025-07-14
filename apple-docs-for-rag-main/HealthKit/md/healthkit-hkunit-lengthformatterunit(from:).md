

- HealthKit
- HKUnit
-  lengthFormatterUnit(from:) 

Type Method

# lengthFormatterUnit(from:)

Converts a HealthKit unit object into a corresponding length formatter enumeration value.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 2.0+

``` source
class func lengthFormatterUnit(from unit: HKUnit) -> LengthFormatter.Unit
```

## Parameters 

`unit`  

A valid HealthKit unit object. If the unit is not a length unit, this method throws an exception (invalidArgumentException).

## Return Value

A length formatter unit value. For a list of possible length formatter unit values see LengthFormatter.Unit.

## See Also

### Working with formatter units

class func energyFormatterUnit(from: HKUnit) -> EnergyFormatter.Unit

Converts a HealthKit unit object into a corresponding energy formatter enumeration value.

convenience init(from: EnergyFormatter.Unit)

Converts an energy formatter enumeration value into a corresponding HealthKit unit object.

convenience init(from: LengthFormatter.Unit)

Converts a length formatter enumeration value into a corresponding HealthKit object.

class func massFormatterUnit(from: HKUnit) -> MassFormatter.Unit

Converts a HealthKit unit object into a corresponding mass formatter enumeration value.

convenience init(from: MassFormatter.Unit)

Converts a mass formatter enumeration value into a corresponding HealthKit unit object.

