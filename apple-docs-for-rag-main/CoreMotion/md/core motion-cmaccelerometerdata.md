

- Core Motion
-  CMAccelerometerData 

Class

# CMAccelerometerData

A data sample from the device’s three accelerometers.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+watchOS 2.0+

``` source
class CMAccelerometerData
```

## Overview

An application accesses `CMAccelerometerData` objects through the block handler specified as the last parameter of the startAccelerometerUpdates(to:withHandler:) method and through the accelerometerData property, both declared by the `CMMotionManager` class. The superclass of `CMAccelerometerData`, CMLogItem, defines a timestamp property that records when the acceleration measurement was taken.

## Topics

### Accessing Accelerometer Data

var acceleration: CMAcceleration

The acceleration measured by the accelerometer.

struct CMAcceleration

The type of a structure containing 3-axis acceleration values.

## Relationships

### Inherits From

- CMLogItem

### Inherited By

- CMRecordedAccelerometerData

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

### Accelerometers

Getting raw accelerometer events

Retrieve data from the onboard accelerometers.

class CMRecordedAccelerometerData

A single piece of accelerometer data that was recorded by the device.

class CMSensorRecorder

An object that gathers and retrieves accelerometer data from a device.

class CMSensorDataList

A list of the accelerometer data recorded by the system.

