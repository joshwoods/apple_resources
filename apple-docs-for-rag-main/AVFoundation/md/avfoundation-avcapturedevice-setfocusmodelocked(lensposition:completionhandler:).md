

- AVFoundation
- AVCaptureDevice
-  setFocusModeLocked(lensPosition:completionHandler:) 

Instance Method

# setFocusModeLocked(lensPosition:completionHandler:)

Locks the lens position at the specified value, and sets the focus mode to a locked state.

iOS 8.0+iPadOS 8.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
func setFocusModeLocked(
    lensPosition: Float,
    completionHandler handler: ((CMTime) -> Void)? = nil
)
```

``` source
func setFocusModeLocked(lensPosition: Float) async -> CMTime
```

## Parameters 

`lensPosition`  

The lens position. Pass a value of currentLensPosition to leave the current lens position unchanged.

`handler`  

A callback the system invokes when the adjustment to the lens position is complete and the focusMode set to a locked state. If you call this method multiple times, the system calls the completion handlers in FIFO order.

The system passes a time value that matches that of the first buffer to which its applied all settings. It synchronizes the timestamp to the device clock, and you must convert the timestamp to the synchronizationClock prior to comparison with the timestamps of buffers delivered through an AVCaptureVideoDataOutput.

You can pass `nil` for this parameter if you don’t require this information.

## Discussion

Calling this method is the only way to set the value of the lensPosition property. This method throws an exception if you set the value to an unsupported level.

Before changing the value the lens position, you must call lockForConfiguration() to acquire exclusive access to the device’s configuration properties. Otherwise, setting the value of this property raises an exception. When you finish configuring the device, call unlockForConfiguration() to release the lock and allow other devices to configure the settings.

## See Also

### Setting Focus Manually

var isLockingFocusWithCustomLensPositionSupported: Bool

A Boolean value that indicates whether the device supports locking focus to a specific lens position.

var lensPosition: Float

The current focus position of the lens.

class let currentLensPosition: Float

A constant that represents the current lens position.

