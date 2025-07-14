

- Core Motion
-  CMOdometerData 

Class

# CMOdometerData

A class that represents odometer data for workouts.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+watchOS 1.0+

``` source
class CMOdometerData
```

## Overview

To get the measurements, use the speed and slope properties. To compute distances, use the deltaDistance and deltaAltitude properties.

## Topics

### Getting speed and slope

var speed: CLLocationSpeed

The instantaneous velocity of the device, measured in meters per second.

var slope: Double?

The slope at the location toward the direction of travel, measured in degrees.

var maxAbsSlope: Double?

The maximum absolute slope at the location toward all directions, measured in degrees.

### Getting date and times

var startDate: Date

The time that the device starts recording the odometer data.

var endDate: Date

The time that the device stops recording the odometer data.

var gpsDate: Date

The time of the GPS measurement associated with the location.

### Measuring distances

var deltaDistance: CLLocationDistance

The change in distance that the user travels since the last location, measured in meters.

var deltaAltitude: CLLocationDistance

The change in altitude above mean sea level associated with the location, measured in meters.

### Getting the location accuracy

var speedAccuracy: CLLocationSpeedAccuracy

The accuracy of the speed value.

var verticalAccuracy: CLLocationAccuracy

The validity of the altitude values and their estimated uncertainty, measured in meters.

var deltaDistanceAccuracy: CLLocationAccuracy

The accuracy of the change in distance value.

### Getting the device

var originDevice: CMOdometerOriginDevice

The device that measures the data.

enum CMOdometerOriginDevice

The device that the odometer sample originates from.

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

### Pedometer and fitness

class CMPedometer

An object for fetching the system-generated live walking data.

class CMPedometerData

Information about the distance traveled by a user on foot.

class CMPedometerEvent

A change in the user’s pedestrian activity.

class CMStepCounter

The number of steps the user has taken with the device.

Deprecated

class CMHighFrequencyHeartRateData

A class that represents heart rate data collected at 1 Hz.

