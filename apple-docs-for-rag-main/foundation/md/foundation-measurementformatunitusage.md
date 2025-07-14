

- Foundation
-  MeasurementFormatUnitUsage 

Structure

# MeasurementFormatUnitUsage

A type that provides the generalized usage for a formatted measurement.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct MeasurementFormatUnitUsage where UnitType : Dimension
```

## Topics

### Selecting a General Format for a Measurement Unit

static var general: MeasurementFormatUnitUsage&lt;UnitType>

A general usage of the formatted measurement.

static var asProvided: MeasurementFormatUnitUsage&lt;UnitType>

A usage of the formatted measurement that reflects the units that you used to create the measurement.

### Selecting a Format for an Energy Measurement

static var food: MeasurementFormatUnitUsage&lt;UnitEnergy>

A usage of an energy measurement related to food.

static var workout: MeasurementFormatUnitUsage&lt;UnitEnergy>

A usage of a energy measurement related to a workout.

### Selecting a Format for a Length Measurement

static var person: MeasurementFormatUnitUsage&lt;UnitLength>

A format usage of a length measurement for displaying a distance as it relates to people.

static var personHeight: MeasurementFormatUnitUsage&lt;UnitLength>

A usage of a length measurement related to a person’s height.

static var road: MeasurementFormatUnitUsage&lt;UnitLength>

A usage of a length measurement related to a road.

### Selecting a Format for a Mass Measurement

static var personWeight: MeasurementFormatUnitUsage&lt;UnitMass>

A usage of a mass measurement related to a person’s weight.

### Selecting a Format for a Temperature Measurement

static var person: MeasurementFormatUnitUsage&lt;UnitTemperature>

A format usage of a temperature measurement for displaying a temperature as it relates to people.

static var weather: MeasurementFormatUnitUsage&lt;UnitTemperature>

A usage of a temperature measurement related to the weather.

### Type Properties

static var barometric: MeasurementFormatUnitUsage&lt;UnitPressure>

static var focalLength: MeasurementFormatUnitUsage&lt;UnitLength>

static var liquid: MeasurementFormatUnitUsage&lt;UnitVolume>

static var rainfall: MeasurementFormatUnitUsage&lt;UnitLength>

static var snowfall: MeasurementFormatUnitUsage&lt;UnitLength>

static var visibility: MeasurementFormatUnitUsage&lt;UnitLength>

static var wind: MeasurementFormatUnitUsage&lt;UnitSpeed>

## Relationships

### Conforms To

- Decodable
- Encodable
- Equatable
- Hashable
- Sendable

