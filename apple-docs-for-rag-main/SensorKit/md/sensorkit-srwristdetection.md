

- SensorKit
-  SRWristDetection 

Class

# SRWristDetection

The configuration of a watch on the wearer’s wrist.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
class SRWristDetection
```

## Overview

The onWristState sensor provides this class as its sample type.

## Topics

### Inspecting Watch Configuration

var crownOrientation: SRWristDetection.CrownOrientation

A value that indicates the direction the Digital Crown faces with respect to the user.

enum CrownOrientation

Directions the Digital Crown can face with respect to the wearer.

var onWrist: Bool

A value that indicates whether the watch is on the user’s wrist.

var onWristDate: Date?

The date and time that the user puts their Apple Watch on their wrist.

var offWristDate: Date?

The date and time that the user takes their Apple Watch off their wrist.

var wristLocation: SRWristDetection.WristLocation

A value that indicates the wrist where the user wears the watch.

enum WristLocation

Preferences for where a user wears a watch.

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

class SRVisit

The user’s progress in their daily travel routine.

