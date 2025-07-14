

- Core Motion
- CMGyroData
-  rotationRate 

Instance Property

# rotationRate

The rotation rate as measured by the device’s gyroscope.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+watchOS 2.0+

``` source
var rotationRate: CMRotationRate { get }
```

## Discussion

This property yields a measurement of the device’s rate of rotation around three axes. Whereas this property gives the raw data from the gyroscope, the identically named property of CMDeviceMotion gives a CMRotationRate structure measuring gyroscope data whose bias has been removed by Core Motion algorithms.

## See Also

### Related Documentation

Event Handling Guide for UIKit Apps

### Getting the Rotation Rate

struct CMRotationRate

The type of structures representing a measurement of rotation rate.

class CMRotationRateData

A data object that contains a single rotation-rate measurement.

class CMRecordedRotationRateData

A data object that contains a single rotation-rate measurement at a specific time.

