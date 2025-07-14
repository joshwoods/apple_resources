

- HealthKit
-  HKUnit 

Class

# HKUnit

A class for managing the units of measure within HealthKit.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 2.0+

``` source
class HKUnit
```

## Mentioned in 

Defining and converting units and quantities

## Overview

The unit class supports most standard SI units (meters, seconds, and grams), SI units with prefixes (centimeters, milliseconds and kilograms) and equivalent non-SI units (feet, minutes, and pounds). HealthKit also supports creating complex units by mathematically combining existing units.

You use units when working with HealthKit quantities. Quantities store both the value (as a `double` data type) and its corresponding unit. You can then request the value from the quantity in any compatible units. For more information on working with quantities, see HKQuantity.

Note

Note

Number formatters that use units (for example, EnergyFormatter, LengthFormatter, and MassFormatter) use a custom enumeration to specify their units. For example, the EnergyFormatter class uses the EnergyFormatter.Unit enum. The HKUnit class provides several methods to translate between the formatter enumerations and the HealthKit units. For more information, see Working with formatter units.

### Using Units

Like many HealthKit classes, the `HKUnit` class is not extendable and should not be subclassed.

The `HKUnit` class is implemented using a facade design pattern. It uses custom subclasses to represent instances of the different unit types. For example, the second() convenience method actually returns an instance of the private `HKTimeUnit` subclass.

Additionally, the unit class uses a single unit instance to represent all copies of the same unit in your app, wherever possible. For example, two calls to the second() method return the same unit object. This helps reduce the amount of memory used by unit instances.

## Topics

### Working with units

convenience init(from: String)

Returns the unit instance described by the provided string.

var unitString: String

A string representation of the unit object.

func isNull() -> Bool

Returns a Boolean value indicating whether the unit is null.

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

convenience init(from: MassFormatter.Unit)

Converts a mass formatter enumeration value into a corresponding HealthKit unit object.

### Constructing mass units

class func gram() -> Self

Returns a HealthKit unit for measuring mass in grams.

class func gramUnit(with: HKMetricPrefix) -> Self

Returns a HealthKit unit for measuring mass, using gram units with the provided prefix.

class func ounce() -> Self

Returns a HealthKit unit for measuring mass in ounces.

class func pound() -> Self

Returns a HealthKit unit for measuring mass in pounds.

class func stone() -> Self

Returns a HealthKit unit for measuring mass in stones.

class func moleUnit(withMolarMass: Double) -> Self

Returns a HealthKit unit for measuring mass in moles for a given molar mass.

class func moleUnit(with: HKMetricPrefix, molarMass: Double) -> Self

Returns a HealthKit unit for measuring mass in moles, with the given prefix and molar mass.

var HKUnitMolarMassBloodGlucose: Double

The molecular mass of blood glucose, typically used to create mole units for blood glucose.

### Constructing length units

class func meter() -> Self

Returns a HealthKit unit for measuring length in meters.

class func meterUnit(with: HKMetricPrefix) -> Self

Returns a HealthKit unit for measuring length, using meter units with the provided prefix.

class func inch() -> Self

Returns a HealthKit unit for measuring length in inches.

class func foot() -> Self

Returns a HealthKit unit for measuring length in feet.

class func yard() -> Self

Returns a HealthKit unit for measuring length in yards.

class func mile() -> Self

Returns a HealthKit unit for measuring length in miles.

### Constructing volume units

class func liter() -> Self

Returns a HealthKit unit for measuring volume in liters.

class func literUnit(with: HKMetricPrefix) -> Self

Returns a HealthKit unit for measuring volume, using liter units with the provided prefix.

class func fluidOunceUS() -> Self

Returns a HealthKit unit for measuring volume in US fluid ounces.

class func fluidOunceImperial() -> Self

Returns a HealthKit unit for measuring volume in imperial fluid ounces.

class func cupUS() -> Self

Returns a HealthKit unit for measuring volume in US cups.

class func cupImperial() -> Self

Returns a HealthKit unit for measuring volume in imperial cups.

class func pintUS() -> Self

Returns a HealthKit unit for measuring volume in US pints.

class func pintImperial() -> Self

Returns a HealthKit unit for measuring volume in imperial pints.

### Constructing pressure units

class func pascal() -> Self

Returns a HealthKit unit for measuring pressure in pascals.

class func pascalUnit(with: HKMetricPrefix) -> Self

Returns a HealthKit unit for measuring pressure, using pascal units with the provided prefix.

class func millimeterOfMercury() -> Self

Returns a HealthKit unit for measuring pressure in millimeters of mercury.

class func inchesOfMercury() -> Self

Returns a HealthKit unit for measuring pressure in inches of mercury.

class func centimeterOfWater() -> Self

Returns a HealthKit unit for measuring pressure in centimeters of water.

class func atmosphere() -> Self

Returns a HealthKit unit for measuring pressure in atmospheres.

class func decibelAWeightedSoundPressureLevel() -> Self

Returns a HealthKit unit for measuring the difference between the local pressure and the ambient atmospheric pressure caused by sound.

### Constructing time units

class func second() -> Self

Returns a HealthKit unit for measuring time in seconds.

class func secondUnit(with: HKMetricPrefix) -> Self

Returns a HealthKit unit for measuring time, using second units with the provided prefix.

class func minute() -> Self

Returns a HealthKit unit for measuring time in minutes.

class func hour() -> Self

Returns a HealthKit unit for measuring time in hours.

class func day() -> Self

Returns a HealthKit unit for measuring time in days.

### Constructing energy units

class func joule() -> Self

Returns a HealthKit unit for measuring energy in joules.

class func jouleUnit(with: HKMetricPrefix) -> Self

Returns a HealthKit unit for measuring energy, using joule units with the provided prefix.

class func kilocalorie() -> Self

Returns a HealthKit unit for measuring energy in kilocalories.

class func largeCalorie() -> Self

Returns a HealthKit unit for measuring energy in large calories (Cal).

class func smallCalorie() -> Self

Returns a HealthKit unit for measuring energy in small calories (cal).

class func calorie() -> Self

Returns a HealthKit unit for measuring energy in calories.

Deprecated

### Constructing power units

class func watt() -> Self

Returns a HealthKit unit for measuring power in watts.

class func wattUnit(with: HKMetricPrefix) -> Self

Returns a HealthKit unit for measuring power, using watt units with the provided prefix.

### Constructing temperature units

class func degreeCelsius() -> Self

Returns a HealthKit unit for measuring temperature in degrees Celsius.

class func degreeFahrenheit() -> Self

Returns a HealthKit unit for measuring temperature in degrees Fahrenheit.

class func kelvin() -> Self

Returns a HealthKit unit for measuring temperature in kelvins.

### Constructing hearing sensitivity units

class func decibelHearingLevel() -> Self

Returns a HealthKit unit for measuring the intensity of a sound.

### Constructing frequency units

class func hertz() -> Self

Returns a HealthKit unit for measuring frequency in hertz.

class func hertzUnit(with: HKMetricPrefix) -> Self

Returns a HealthKit unit for measuring frequency in hertz with the provided prefix.

### Constructing vision units

class func diopter() -> Self

Returns a HealthKit unit for measuring the optical power of a lens using diopter units.

class func prismDiopter() -> Self

Returns a HealthKit unit for measuring the prismatic deviation of a lens using prism diopter units.

### Constructing angle units

class func degreeAngle() -> Self

Returns a HealthKit unit for measuring angles using degrees.

class func radianAngle() -> Self

Returns a HealthKit unit for measuring angles using radians.

class func radianAngleUnit(with: HKMetricPrefix) -> Self

Returns a HealthKit unit for measuring angles, using radian units with the provided prefix.

### Constructing electrical conductance units

class func siemen() -> Self

Returns a HealthKit unit for measuring electrical conductance in siemens.

class func siemenUnit(with: HKMetricPrefix) -> Self

Returns a HealthKit unit for measuring electrical conductance, using siemen units with the provided prefix.

### Electrical potential difference

class func volt() -> Self

Returns a HealthKit unit for measuring the difference in electrical potential using volts.

class func voltUnit(with: HKMetricPrefix) -> Self

Returns a HealthKit unit for measuring the electrical potential difference in volts with the provided prefix.

### Constructing pharmacology units

class func internationalUnit() -> Self

Returns a HealthKit unit that measures the amount of a biologically active substance in international units (IU).

### Constructing scalar units

class func count() -> Self

Returns a HealthKit unit for measuring counts.

class func percent() -> Self

Returns a HealthKit unit for measuring percentages.

### Performing unit math

func unitMultiplied(by: HKUnit) -> HKUnit

Creates a complex unit by multiplying the receiving unit with another unit.

func unitDivided(by: HKUnit) -> HKUnit

Creates a complex unit by dividing the receiving unit by another unit.

func unitRaised(toPower: Int) -> HKUnit

Creates a complex unit by raising the unit to the given power.

func reciprocal() -> HKUnit

Returns a complex unit representing the unit’s reciprocal.

### Constants

enum HKMetricPrefix

Prefixes that can be added to SI units to change the order of magnitude.

### Type Methods

class func appleEffortScore() -> Self

class func lux() -> Self

class func luxUnit(with: HKMetricPrefix) -> Self

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding
- Sendable

## See Also

### Units and quantities

Defining and converting units and quantities

Create and convert units and quantities.

class HKQuantity

An object that stores a value for a given unit.

enum HKMetricPrefix

Prefixes that can be added to SI units to change the order of magnitude.

