

- EventKit
-  EKAlarm 

Class

# EKAlarm

A class that represents an alarm.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.8+visionOS 1.0+watchOS 2.0+

``` source
class EKAlarm
```

## Overview

An EKAlarm object represents an alarm in Event Kit. Use the init(absoluteDate:) and init(relativeOffset:) class methods to create an alarm and use the properties to set information about an alarm. In macOS Mountain Lion, you can specify an action to trigger when the alarm fires via the `emailAddress`, `soundName`, or `url` property.

## Topics

### Creating an Alarm

init(absoluteDate: Date)

Creates and returns an alarm with an absolute date.

init(relativeOffset: TimeInterval)

Creates and returns an alarm with a relative offset.

### Accessing Alarm Dates

var absoluteDate: Date?

The absolute date for the alarm.

var relativeOffset: TimeInterval

The offset from the start of an event, at which the alarm fires.

### Setting GeoFence-based Alarms

enum EKAlarmProximity

A value indicating whether an alarm is triggered by entering or exiting a region.

var proximity: EKAlarmProximity

A value indicating how a location-based alarm is triggered.

var structuredLocation: EKStructuredLocation?

The location to trigger an alarm.

### Triggering Alarm Actions

These properties are only available in macOS 10.8 or later.

enum EKAlarmType

A value that specifies what type of action occurs when the alarm triggers.

var type: EKAlarmType

The type of action to trigger when the alarm fires.

var emailAddress: String?

The recipient of an email to send when the alarm triggers.

var soundName: String?

The name of the sound to play when the alarm triggers.

## Relationships

### Inherits From

- EKObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

## See Also

### Alarms

Setting an alarm

Alert users of events and reminders with an alarm.

class EKStructuredLocation

`A` class that specifies a geofence to activate the alarm of a calendar item.

