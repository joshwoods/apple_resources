

- Core Motion
-  CMAbsoluteAltitudeData 

Class

# CMAbsoluteAltitudeData

Data that records a change in absolute altitude.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+visionOS 1.0+watchOS 8.0+

``` source
class CMAbsoluteAltitudeData
```

## Overview

Absolute altitude is only available on iPhone 12 and later and Apple Watch 6 or SE and later.

## Topics

### Accessing Altitude Data

var altitude: Double

The absolute altitude of the device relative to sea level, measured in meters.

var accuracy: Double

The estimated uncertainty of the altimeter in meters, based on one standard deviation.

var precision: Double

The recommended resolution for the altitude, in meters.

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

class CMAltitudeData

Data for a recorded change in altitude.

