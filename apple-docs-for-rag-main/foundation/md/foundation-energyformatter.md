

- Foundation
-  EnergyFormatter 

Class

# EnergyFormatter

A formatter that provides localized descriptions of energy values.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class EnergyFormatter
```

## Overview

Note

As of iOS 10, macOS 10.12, tvOS 10, and watchOS 3, Foundation provides the MeasurementFormatter class, which can be used to represent quantities of UnitEnergy to provide equivalent functionality to EnergyFormatter. You are encouraged to transition to these new Foundation Units and Measurements APIs whenever possible.

## Topics

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

func unitString(fromValue: Double, unit: EnergyFormatter.Unit) -> String

Returns the unit string based on the provided value and unit.

var unitStyle: Formatter.UnitStyle

The unit style used by this formatter.

### Constants

enum Unit

The units supported by the `NSEnergyFormatter` class.

## Relationships

### Inherits From

- Formatter

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol

## See Also

### Deprecated

class LengthFormatter

A formatter that provides localized descriptions of linear distances, such as length and height measurements.

class MassFormatter

A formatter that provides localized descriptions of mass and weight values.

