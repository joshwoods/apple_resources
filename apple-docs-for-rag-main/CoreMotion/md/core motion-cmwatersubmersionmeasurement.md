

- Core Motion
-  CMWaterSubmersionMeasurement 

Class

# CMWaterSubmersionMeasurement

An update that contains data about the pressure and depth.

iOS 16.0+iPadOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
class CMWaterSubmersionMeasurement
```

## Topics

### Accessing the data

var date: Date

The time and date when the system recorded the measurements.

var depth: Measurement&lt;UnitLength>?

The depth under water.

var pressure: Measurement&lt;UnitPressure>?

The water pressure.

var surfacePressure: Measurement&lt;UnitPressure>

The surface air pressure.

var submersionState: CMWaterSubmersionMeasurement.DepthState

The depth state.

enum DepthState

A state based on the device’s depth under water.

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

class CMWaterTemperature

An update that contains data about the water temperature.

