

- AVFoundation
- AVCaptureDevice
-  currentLensPosition 

Type Property

# currentLensPosition

A constant that represents the current lens position.

iOS 8.0+iPadOS 8.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
class let currentLensPosition: Float
```

## Discussion

Pass this value to the setFocusModeLocked(lensPosition:completionHandler:) method to lock focus without changing the current lens position.

## See Also

### Setting Focus Manually

var isLockingFocusWithCustomLensPositionSupported: Bool

A Boolean value that indicates whether the device supports locking focus to a specific lens position.

var lensPosition: Float

The current focus position of the lens.

func setFocusModeLocked(lensPosition: Float, completionHandler: ((CMTime) -> Void)?)

Locks the lens position at the specified value, and sets the focus mode to a locked state.

