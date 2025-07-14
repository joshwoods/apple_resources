

- AVFoundation
- AVCaptureDevice
-  isLockingFocusWithCustomLensPositionSupported 

Instance Property

# isLockingFocusWithCustomLensPositionSupported

A Boolean value that indicates whether the device supports locking focus to a specific lens position.

iOS 10.0+iPadOS 10.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
var isLockingFocusWithCustomLensPositionSupported: Bool { get }
```

## Discussion

If this property’s value is false, calling the setFocusModeLocked(lensPosition:completionHandler:) method with a lens position value other than currentLensPosition raises an exception.

## See Also

### Setting Focus Manually

var lensPosition: Float

The current focus position of the lens.

class let currentLensPosition: Float

A constant that represents the current lens position.

func setFocusModeLocked(lensPosition: Float, completionHandler: ((CMTime) -> Void)?)

Locks the lens position at the specified value, and sets the focus mode to a locked state.

