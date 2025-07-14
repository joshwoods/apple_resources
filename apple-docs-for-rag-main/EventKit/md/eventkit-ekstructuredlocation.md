

- EventKit
-  EKStructuredLocation 

Class

# EKStructuredLocation

`A` class that specifies a geofence to activate the alarm of a calendar item.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.8+visionOS 1.0+watchOS 2.0+

``` source
class EKStructuredLocation
```

## Overview

Use init(title:) to create a new structured location, then set it to the structuredLocation property of an EKAlarm object.

## Topics

### Creating Structured Locations

convenience init(title: String)

Creates a new structured location with the specified title.

convenience init(mapItem: MKMapItem)

Creates a new structured location with the specified map item.

### Accessing Structured Location Properties

var title: String?

The title of the location.

var geoLocation: CLLocation?

The core location.

var radius: Double

A minimum distance from the core location that would trigger the alarm or reminder.

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

class EKAlarm

A class that represents an alarm.

