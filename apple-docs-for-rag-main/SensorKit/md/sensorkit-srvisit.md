

- SensorKit
-  SRVisit 

Class

# SRVisit

The user’s progress in their daily travel routine.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
class SRVisit
```

## Overview

The visits sensor provides this class as its sample type.

## Topics

### Identifying a Visit

var identifier: UUID

A value that maps to a unique geographic location.

### Accessing Visit Information

var arrivalDateInterval: DateInterval

A range of time within which the user arrives at a location of interest.

var departureDateInterval: DateInterval

A range of time within which the user departs from a location of interest.

var distanceFromHome: CLLocationDistance

The location’s distance from the home-category location.

var locationCategory: SRVisit.LocationCategory

The location’s type.

enum LocationCategory

Types of locations.

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

class SRAmbientLightSample

The amount of ambient light in the user’s environment.

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

class SRWristDetection

The configuration of a watch on the wearer’s wrist.

