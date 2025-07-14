

- SensorKit
-  SRMediaEvent 

Class

# SRMediaEvent

A user interaction with a media object, such as an image or a video.

iOS 16.4+iPadOS 16.4+Mac Catalyst 16.4+

``` source
class SRMediaEvent
```

## Topics

### Identifying Media Objects

var mediaIdentifier: String

A unique identifier for the media object.

### Tracking Media Events

var eventType: SRMediaEventType

The type of user interaction with the media.

enum SRMediaEventType

The types of user interaction with media that the sensor tracks.

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

### Interpreting data

class SRAmbientLightSample

The amount of ambient light in the user’s environment.

class SRDeviceUsageReport

The frequency and relative duration that the user uses their device, particular Apple apps, or websites.

class SRKeyboardMetrics

The configuration of a device’s keyboard and its usage patterns.

class SRMessagesUsageReport

An object that describes the user’s Messages app activity over a period of time.

class SRPhoneUsageReport

An object that describes the user’s phone activity over a period of time.

class SRVisit

The user’s progress in their daily travel routine.

class SRWristDetection

The configuration of a watch on the wearer’s wrist.

