

- Core Motion
- CMMotionManager
-  isDeviceMotionAvailable 

Instance Property

# isDeviceMotionAvailable

A Boolean value that indicates whether the device-motion service is available on the device.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+visionOS 1.0+watchOS 2.0+

``` source
var isDeviceMotionAvailable: Bool { get }
```

## Mentioned in 

Getting processed device-motion data

## Discussion

The device-motion service is available if a device has both an accelerometer and a gyroscope. Because all devices have accelerometers, this property is functionally equivalent to isGyroAvailable.

## See Also

### Related Documentation

var isDeviceMotionActive: Bool

A Boolean value that determines whether the app is receiving updates from the device-motion service.

### Determining the Availability of Services

var isAccelerometerAvailable: Bool

A Boolean value that indicates whether an accelerometer is available on the device.

var isGyroAvailable: Bool

A Boolean value that indicates whether a gyroscope is available on the device.

var isMagnetometerAvailable: Bool

A Boolean value that indicates whether a magnetometer is available on the device.

