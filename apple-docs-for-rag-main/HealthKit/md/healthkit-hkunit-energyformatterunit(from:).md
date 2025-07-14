

- HealthKit
- HKUnit
-  energyFormatterUnit(from:) 

Type Method

# energyFormatterUnit(from:)

Converts a HealthKit unit object into a corresponding energy formatter enumeration value.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 2.0+

``` source
class func energyFormatterUnit(from unit: HKUnit) -> EnergyFormatter.Unit
```

## Parameters 

`unit`  

A valid HealthKit unit object. If the unit is not an energy-type unit, this method throws an exception (invalidArgumentException).

## Return Value

An energy formatter unit value. For a list of possible energy formatter unit values, see EnergyFormatter.Unit.

## See Also

### Working with formatter units

convenience init(from: EnergyFormatter.Unit)

Converts an energy formatter enumeration value into a corresponding HealthKit unit object.

class func lengthFormatterUnit(from: HKUnit) -> LengthFormatter.Unit

Converts a HealthKit unit object into a corresponding length formatter enumeration value.

convenience init(from: LengthFormatter.Unit)

Converts a length formatter enumeration value into a corresponding HealthKit object.

class func massFormatterUnit(from: HKUnit) -> MassFormatter.Unit

Converts a HealthKit unit object into a corresponding mass formatter enumeration value.

convenience init(from: MassFormatter.Unit)

Converts a mass formatter enumeration value into a corresponding HealthKit unit object.

