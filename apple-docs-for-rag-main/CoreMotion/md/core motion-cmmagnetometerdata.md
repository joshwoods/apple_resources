

- Core Motion
-  CMMagnetometerData 

Class

# CMMagnetometerData

Measurements of the Earth’s magnetic field relative to the device.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.15+watchOS 2.0+

``` source
class CMMagnetometerData
```

## Overview

Your application can obtain samples of magnetometer measurements, as represented by instances of this class, from the block handler of the startMagnetometerUpdates(to:withHandler:) method or from the magnetometerData property of the `CMMotionManager` class.

Note

The magnetometerData property of `CMMotionManager` provides a non-`nil` value only if you have called the `startMagnetometerUpdates()` method or the startMagnetometerUpdates(to:withHandler:) method to start magnetometer updates.

## Topics

### Getting the Field Strength

var magneticField: CMMagneticField

Returns the magnetic field measured by the magnetometer.

struct CMMagneticField

A structure containing 3-axis magnetometer data

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

