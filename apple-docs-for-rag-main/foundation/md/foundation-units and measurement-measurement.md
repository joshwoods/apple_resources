

- Foundation
-  Units and Measurement 

API Collection

# Units and Measurement

Label numeric quantities with physical dimensions to allow locale-aware formatting and conversion between related units.

## Topics

### Essentials

struct Measurement

A numeric quantity labeled with a unit of measure, with support for unit conversion and unit-aware calculations.

class NSMeasurement

A numeric quantity labeled with a unit of measure, with support for unit conversion and unit-aware calculations.

class Unit

An abstract class representing a unit of measure.

class Dimension

An abstract class representing a dimensional unit of measure.

### Conversion

class UnitConverter

An abstract class that provides a description of how to convert a unit to and from the base unit of its dimension.

class UnitConverterLinear

A description of how to convert between units using a linear equation.

### Physical Dimension

class UnitArea

A unit of measure for area.

class UnitLength

A unit of measure for length.

class UnitVolume

A unit of measure for volume.

class UnitAngle

A unit of measure for planar angle and rotation.

### Mass, Weight, and Force

class UnitMass

A unit of measure for mass.

class UnitPressure

A unit of measure for pressure.

### Time and Motion

class UnitAcceleration

A unit of measure for acceleration.

class UnitDuration

A unit of measure for a duration of time.

class UnitFrequency

A unit of measure for frequency.

class UnitSpeed

A unit of measure for speed.

### Energy, Heat, and Light

class UnitEnergy

A unit of measure for energy.

class UnitPower

A unit of measure for power.

class UnitTemperature

A unit of measure for temperature.

class UnitIlluminance

A unit of measure for illuminance.

### Electricity

class UnitElectricCharge

A unit of measure for electric charge.

class UnitElectricCurrent

A unit of measure for electric current.

class UnitElectricPotentialDifference

A unit of measure for electric potential difference.

class UnitElectricResistance

A unit of measure for electric resistance.

### Concentration and Dispersion

class UnitConcentrationMass

A unit of measure for concentration of mass.

class UnitDispersion

A unit of measure for specific quantities of dispersion.

### Fuel Efficiency

class UnitFuelEfficiency

A unit of measure for fuel efficiency.

### Data Storage

class UnitInformationStorage

A unit of measure for quantities of information.

### Formatting Measurements

struct MeasurementFormatUnitUsage

A type that provides the generalized usage for a formatted measurement.

## See Also

### Fundamentals

Numbers, Data, and Basic Values

Work with primitive values and other fundamental types used throughout Cocoa.

Strings and Text

Create and process strings of Unicode characters, use regular expressions to find patterns, and perform natural language analysis of text.

Collections

Use arrays, dictionaries, sets, and specialized collections to store and iterate groups of objects or values.

Dates and Times

Compare dates and times, and perform calendar and time zone calculations.

Data Formatting

Convert numbers, dates, measurements, and other values to and from locale-aware string representations.

Filters and Sorting

Use predicates, expressions, and sort descriptors to examine elements in collections and other services.

