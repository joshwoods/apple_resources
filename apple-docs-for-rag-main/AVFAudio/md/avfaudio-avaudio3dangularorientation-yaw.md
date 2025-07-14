

- AVFAudio
- AVAudio3DAngularOrientation
-  yaw 

Instance Property

# yaw

The side-to-side movement of the listener’s head.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var yaw: Float
```

## Discussion

The yaw axis describes the side-to-side movement of the listener’s head, and is perpendicular to the plane of the listener’s ears. Its origin is at the center of the listener’s head and points toward the bottom of the head. A positive yaw is in the clockwise direction going from `0` to `180` degrees. A negative yaw is in the counterclockwise direction going from `0` to `-180` degrees.

## See Also

### Getting Angular Orientation Properties

var pitch: Float

The up-and-down movement of the listener’s head.

var roll: Float

The tilt of the listener’s head.

