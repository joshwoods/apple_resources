

- HealthKit
- HKUnit
-  massFormatterUnit(from:) 

Type Method

# massFormatterUnit(from:)

Converts a HealthKit unit object into a corresponding mass formatter enumeration value.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 2.0+

``` source
class func massFormatterUnit(from unit: HKUnit) -> MassFormatter.Unit
```

## Parameters 

`unit`  

A valid HealthKit unit object. If the unit is not a mass-type unit, this method throws an exception (invalidArgumentException).

## Return Value

A mass formatter unit value. For a list of possible mass formatter unit values, see MassFormatter.Unit.

## See Also

### Working with formatter units

class func energyFormatterUnit(from: HKUnit) -> EnergyFormatter.Unit

Converts a HealthKit unit object into a corresponding energy formatter enumeration value.

convenience init(from: EnergyFormatter.Unit)

Converts an energy formatter enumeration value into a corresponding HealthKit unit object.

class func lengthFormatterUnit(from: HKUnit) -> LengthFormatter.Unit

Converts a HealthKit unit object into a corresponding length formatter enumeration value.

convenience init(from: LengthFormatter.Unit)

Converts a length formatter enumeration value into a corresponding HealthKit object.

convenience init(from: MassFormatter.Unit)

Converts a mass formatter enumeration value into a corresponding HealthKit unit object.

