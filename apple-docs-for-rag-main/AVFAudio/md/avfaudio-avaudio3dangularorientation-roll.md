

- AVFAudio
- AVAudio3DAngularOrientation
-  roll 

Instance Property

# roll

The tilt of the listener’s head.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var roll: Float
```

## Discussion

The roll axis describes the tilt of the listener’s head, and is perpendicular to the other two axes. Its origin is at the center of the listener’s head and points toward the listener’s nose. A positive roll is to the right going from `0` to `180` degrees. A negative roll is to the left going from `0` to `-180` degrees.

## See Also

### Getting Angular Orientation Properties

var yaw: Float

The side-to-side movement of the listener’s head.

var pitch: Float

The up-and-down movement of the listener’s head.

