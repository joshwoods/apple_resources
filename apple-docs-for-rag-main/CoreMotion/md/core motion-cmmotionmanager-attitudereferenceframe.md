

- Core Motion
- CMMotionManager
-  attitudeReferenceFrame 

Instance Property

# attitudeReferenceFrame

Returns either the reference frame currently being used or the default attitude reference frame.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+visionOS 1.0+watchOS 2.0+

``` source
var attitudeReferenceFrame: CMAttitudeReferenceFrame { get }
```

## Mentioned in 

Getting processed device-motion data

## Discussion

If the device-motion service is active, this property returns the reference frame currently in use. If the service is inactive, but your app started it at some point since launch, this property contains the last reference frame you used. If you haven’t started the device-motion service since app launch, this property returns the default frame of reference, which is xArbitraryZVertical.

If device motion is not available on the current device, the value of this property is undefined.

## See Also

### Related Documentation

var isDeviceMotionAvailable: Bool

A Boolean value that indicates whether the device-motion service is available on the device.

### Accessing Attitude Reference Frames

class func availableAttitudeReferenceFrames() -> CMAttitudeReferenceFrame

Returns a bitmask of the available reference frames for reporting the attitude of the current device.

