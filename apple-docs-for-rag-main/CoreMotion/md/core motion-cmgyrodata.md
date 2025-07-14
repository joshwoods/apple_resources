

- Core Motion
-  CMGyroData 

Class

# CMGyroData

A single measurement of the device’s rotation rate.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+watchOS 2.0+

``` source
class CMGyroData
```

## Overview

An application receives or samples `CMGyroData` objects at regular intervals after calling the startGyroUpdates(to:withHandler:) method or the startGyroUpdates() method of the CMMotionManager class.

## Topics

### Getting the Rotation Rate

var rotationRate: CMRotationRate

The rotation rate as measured by the device’s gyroscope.

struct CMRotationRate

The type of structures representing a measurement of rotation rate.

class CMRotationRateData

A data object that contains a single rotation-rate measurement.

class CMRecordedRotationRateData

A data object that contains a single rotation-rate measurement at a specific time.

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

### Gyroscopes

Getting raw gyroscope events

Retrieve data from the onboard gyroscopes.

