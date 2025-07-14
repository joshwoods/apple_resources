

- Core Motion
- CMMotionManager
-  isMagnetometerActive 

Instance Property

# isMagnetometerActive

A Boolean value that determines whether magnetometer updates are currently happening.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+watchOS 2.0+

``` source
var isMagnetometerActive: Bool { get }
```

## Discussion

This property indicates whether the startMagnetometerUpdates(to:withHandler:) or startMagnetometerUpdates() method has been called since the last time the stopMagnetometerUpdates() method was called. (If the start methods hadn’t been called, the app could be getting updates from the magnetometer after calling, for example, startDeviceMotionUpdates(), but this property would return false.)

## See Also

### Related Documentation

var isMagnetometerAvailable: Bool

A Boolean value that indicates whether a magnetometer is available on the device.

### Determining Which Services Are Active

var isDeviceMotionActive: Bool

A Boolean value that determines whether the app is receiving updates from the device-motion service.

var isAccelerometerActive: Bool

A Boolean value that indicates whether accelerometer updates are currently happening.

var isGyroActive: Bool

A Boolean value that determines whether gyroscope updates are currently happening.

