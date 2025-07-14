

- Core Motion
-  CMLogItem 

Class

# CMLogItem

The base class for all motion-related data objects.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+watchOS 2.0+

``` source
class CMLogItem
```

## Overview

The `CMLogItem` class defines a read-only timestamp property that records the time a motion-event measurement was taken.

## Topics

### Getting the Time of the Event

var timestamp: TimeInterval

The time when the logged item is valid.

## Relationships

### Inherits From

- NSObject

### Inherited By

- CMAbsoluteAltitudeData
- CMAccelerometerData
- CMAltitudeData
- CMAmbientPressureData
- CMDeviceMotion
- CMGyroData
- CMHighFrequencyHeartRateData
- CMMagnetometerData
- CMMotionActivity
- CMRotationRateData

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

