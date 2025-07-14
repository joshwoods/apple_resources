

- Core Motion
- CMMotionManager
-  isAccelerometerActive 

Instance Property

# isAccelerometerActive

A Boolean value that indicates whether accelerometer updates are currently happening.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+visionOS 1.0+watchOS 2.0+

``` source
var isAccelerometerActive: Bool { get }
```

## Discussion

This property indicates whether startAccelerometerUpdates(to:withHandler:) or startAccelerometerUpdates() has been called since the last time stopAccelerometerUpdates() was called. (If the start methods hadn’t been called, the app could be getting updates from the accelerometer after calling, for example, startDeviceMotionUpdates(), but this property would return false.)

## See Also

### Related Documentation

var isAccelerometerAvailable: Bool

A Boolean value that indicates whether an accelerometer is available on the device.

### Determining Which Services Are Active

var isDeviceMotionActive: Bool

A Boolean value that determines whether the app is receiving updates from the device-motion service.

var isGyroActive: Bool

A Boolean value that determines whether gyroscope updates are currently happening.

var isMagnetometerActive: Bool

A Boolean value that determines whether magnetometer updates are currently happening.

