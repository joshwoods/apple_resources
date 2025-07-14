

- Core Motion
- CMMotionManager
-  availableAttitudeReferenceFrames() 

Type Method

# availableAttitudeReferenceFrames()

Returns a bitmask of the available reference frames for reporting the attitude of the current device.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+visionOS 1.0+watchOS 2.0+

``` source
class func availableAttitudeReferenceFrames() -> CMAttitudeReferenceFrame
```

## Return Value

A bitmask that you can bitwise-AND with the `enum` constants of the CMAttitudeReferenceFrame type.

## Discussion

When starting a service that allows you to specify a reference frame, it’s your responsibility to specify a reference frame that’s available on the current device. Some reference frames might be unavailable because the required hardware isn’t present or not currently available.

The following example shows how to call this method and test for the availability of the xMagneticNorthZVertical value.

```
```

## See Also

### Accessing Attitude Reference Frames

var attitudeReferenceFrame: CMAttitudeReferenceFrame

Returns either the reference frame currently being used or the default attitude reference frame.

