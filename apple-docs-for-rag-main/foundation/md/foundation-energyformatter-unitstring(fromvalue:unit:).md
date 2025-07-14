

- Foundation
- EnergyFormatter
-  unitString(fromValue:unit:) 

Instance Method

# unitString(fromValue:unit:)

Returns the unit string based on the provided value and unit.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func unitString(
    fromValue value: Double,
    unit: EnergyFormatter.Unit
) -> String
```

## Parameters 

`value`  

The energy value in the provided unit.

`unit`  

The unit to use in the resulting energy string.

## Return Value

A localized string representing the given unit. The provided value determines whether the unit is plural or singular.

## See Also

### Formatting Energy Strings

var isForFoodEnergyUse: Bool

A Boolean value that indicates whether the energy value is used to measure food energy.

func getObjectValue(AutoreleasingUnsafeMutablePointer&lt;AnyObject?>?, for: String, errorDescription: AutoreleasingUnsafeMutablePointer&lt;NSString?>?) -> Bool

This method is not supported for the `NSEnergyFormatter` class.

var numberFormatter: NumberFormatter!

The number formatter used to format the numbers in energy strings.

func string(fromJoules: Double) -> String

Returns an energy string for the provided value.

func string(fromValue: Double, unit: EnergyFormatter.Unit) -> String

Returns a properly formatted energy string for the given value and unit.

func unitString(fromJoules: Double, usedUnit: UnsafeMutablePointer&lt;EnergyFormatter.Unit>?) -> String

Returns the unit string for the provided value.

var unitStyle: Formatter.UnitStyle

The unit style used by this formatter.

