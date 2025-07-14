

- AVFoundation
- AVCaptureDevice
-  lensPosition 

Instance Property

# lensPosition

The current focus position of the lens.

iOS 8.0+iPadOS 8.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
var lensPosition: Float { get }
```

## Discussion

A lens position value doesn’t correspond to an exact physical distance, nor does it represent a consistent focus distance from device to device.

The range of possible positions is `0.0` to `1.0`, with `0.0` being the shortest distance at which the lens can focus and `1.0` the furthest. Note that `1.0` doesn’t represent focus at infinity. The default value is `1.0`.

This property is key-value observable.

## See Also

### Setting Focus Manually

var isLockingFocusWithCustomLensPositionSupported: Bool

A Boolean value that indicates whether the device supports locking focus to a specific lens position.

class let currentLensPosition: Float

A constant that represents the current lens position.

func setFocusModeLocked(lensPosition: Float, completionHandler: ((CMTime) -> Void)?)

Locks the lens position at the specified value, and sets the focus mode to a locked state.

