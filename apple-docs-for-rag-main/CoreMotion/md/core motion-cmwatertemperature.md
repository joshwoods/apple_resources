

- Core Motion
-  CMWaterTemperature 

Class

# CMWaterTemperature

An update that contains data about the water temperature.

iOS 16.0+iPadOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
class CMWaterTemperature
```

## Topics

### Accessing the data

var date: Date

The time and date when the system recorded the measurements.

var temperature: Measurement&lt;UnitTemperature>

The water temperature.

var temperatureUncertainty: Measurement&lt;UnitTemperature>

The amount of uncertainty in the measurement of the water temperature.

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

## See Also

### Water submersion

Accessing submersion data

Use a water-submersion manager to receive water pressure, temperature, and depth data on Apple Watch Ultra.

class CMWaterSubmersionManager

An object for managing the collection of pressure and temperature data during submersion.

protocol CMWaterSubmersionManagerDelegate

A delegate that receives updates about ambient pressure, water pressure, water temperature, and submersion events.

class CMWaterSubmersionEvent

An event indicating that the device’s submersion state has changed.

class CMWaterSubmersionMeasurement

An update that contains data about the pressure and depth.

