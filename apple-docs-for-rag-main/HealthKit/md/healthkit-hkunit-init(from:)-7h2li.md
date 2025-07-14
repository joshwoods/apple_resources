

- HealthKit
- HKUnit
-  init(from:) 

Initializer

# init(from:)

Converts a mass formatter enumeration value into a corresponding HealthKit unit object.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 2.0+

``` source
convenience init(from massFormatterUnit: MassFormatter.Unit)
```

## Parameters 

`massFormatterUnit`  

A valid mass formatter unit value. For a list of possible mass formatter unit values, see MassFormatter.Unit.

## Return Value

A HealthKit unit object, or `nil` if the unit parameter is not a valid energy formatter unit value.

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

class func massFormatterUnit(from: HKUnit) -> MassFormatter.Unit

Converts a HealthKit unit object into a corresponding mass formatter enumeration value.

