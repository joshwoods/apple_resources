

- SensorKit
-  SRAmbientLightSample 

Class

# SRAmbientLightSample

The amount of ambient light in the user’s environment.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
class SRAmbientLightSample
```

## Overview

The ambientLightSensor sensor provides this class as its sample type.

## Topics

### Measuring light level

var chromaticity: SRAmbientLightSample.Chromaticity

A coordinate pair that describes the sample’s light brightness and tint.

struct Chromaticity

A coordinate pair that describes light brightness and tint.

var lux: Measurement&lt;UnitIlluminance>

An object that describes the sample’s luminous flux.

var placement: SRAmbientLightSample.SensorPlacement

The light’s location relative to the sensor.

enum SensorPlacement

Directional values that describe light-source location with respect to the sensor.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Interpreting data

class SRDeviceUsageReport

The frequency and relative duration that the user uses their device, particular Apple apps, or websites.

class SRKeyboardMetrics

The configuration of a device’s keyboard and its usage patterns.

class SRMediaEvent

A user interaction with a media object, such as an image or a video.

class SRMessagesUsageReport

An object that describes the user’s Messages app activity over a period of time.

class SRPhoneUsageReport

An object that describes the user’s phone activity over a period of time.

class SRVisit

The user’s progress in their daily travel routine.

class SRWristDetection

The configuration of a watch on the wearer’s wrist.

