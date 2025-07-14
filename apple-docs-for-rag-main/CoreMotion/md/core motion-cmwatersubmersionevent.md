

- Core Motion
-  CMWaterSubmersionEvent 

Class

# CMWaterSubmersionEvent

An event indicating that the device’s submersion state has changed.

iOS 16.0+iPadOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
class CMWaterSubmersionEvent
```

## Topics

### Accessing event data

var date: Date

The time and date of the event.

var state: CMWaterSubmersionEvent.State

The new submersion state.

enum State

The device’s submersion state.

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

class CMWaterSubmersionMeasurement

An update that contains data about the pressure and depth.

class CMWaterTemperature

An update that contains data about the water temperature.

