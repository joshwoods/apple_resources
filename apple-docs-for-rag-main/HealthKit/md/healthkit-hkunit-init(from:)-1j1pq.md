

- HealthKit
- HKUnit
-  init(from:) 

Initializer

# init(from:)

Converts an energy formatter enumeration value into a corresponding HealthKit unit object.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 2.0+

``` source
convenience init(from energyFormatterUnit: EnergyFormatter.Unit)
```

## Parameters 

`energyFormatterUnit`  

A valid energy formatter unit value. For a list of possible energy formatter unit values, see EnergyFormatter.Unit.

## Return Value

A HealthKit unit object, or `nil` if the unit parameter is not a valid energy formatter unit value.

## See Also

### Working with formatter units

class func energyFormatterUnit(from: HKUnit) -> EnergyFormatter.Unit

Converts a HealthKit unit object into a corresponding energy formatter enumeration value.

class func lengthFormatterUnit(from: HKUnit) -> LengthFormatter.Unit

Converts a HealthKit unit object into a corresponding length formatter enumeration value.

convenience init(from: LengthFormatter.Unit)

Converts a length formatter enumeration value into a corresponding HealthKit object.

class func massFormatterUnit(from: HKUnit) -> MassFormatter.Unit

Converts a HealthKit unit object into a corresponding mass formatter enumeration value.

convenience init(from: MassFormatter.Unit)

Converts a mass formatter enumeration value into a corresponding HealthKit unit object.

