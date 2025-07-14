

- Core Motion
- CMMotionManager
-  isDeviceMotionActive 

Instance Property

# isDeviceMotionActive

A Boolean value that determines whether the app is receiving updates from the device-motion service.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+visionOS 1.0+watchOS 2.0+

``` source
var isDeviceMotionActive: Bool { get }
```

## Discussion

This property indicates whether startDeviceMotionUpdates(to:withHandler:) or startDeviceMotionUpdates() has been called since the last time stopDeviceMotionUpdates() was called.

## See Also

### Related Documentation

var isDeviceMotionAvailable: Bool

A Boolean value that indicates whether the device-motion service is available on the device.

### Determining Which Services Are Active

var isAccelerometerActive: Bool

A Boolean value that indicates whether accelerometer updates are currently happening.

var isGyroActive: Bool

A Boolean value that determines whether gyroscope updates are currently happening.

var isMagnetometerActive: Bool

A Boolean value that determines whether magnetometer updates are currently happening.

