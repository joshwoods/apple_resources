

- Core Motion
-  CMAltitudeData 

Class

# CMAltitudeData

Data for a recorded change in altitude.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+watchOS 2.0+

``` source
class CMAltitudeData
```

## Overview

You do not create instances of this class directly. When you want to receive altimeter changes, create an instance of the CMAltimeter class and use that object to query for events or to start the delivery of events. The altimeter object creates new instances of this class at appropriate times and delivers them to the handler you specify.

## Topics

### Getting the Altitude Data

var relativeAltitude: NSNumber

The change in altitude (in meters) since the first reported event.

var pressure: NSNumber

The recorded pressure, in kilopascals.

## Relationships

### Inherits From

- CMLogItem

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

### Altitude data

class CMAltimeter

An object that initiates the delivery of altitude-related changes.

class CMAbsoluteAltitudeData

Data that records a change in absolute altitude.

