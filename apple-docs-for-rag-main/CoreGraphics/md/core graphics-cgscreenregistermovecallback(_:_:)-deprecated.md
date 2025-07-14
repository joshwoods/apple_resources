

- Core Graphics
-  CGScreenRegisterMoveCallback(\_:\_:) Deprecated

Function

# CGScreenRegisterMoveCallback(\_:\_:)

Registers a callback function to be invoked when an area of the display is moved.

Mac Catalyst 13.1–13.1Deprecated

``` source
func CGScreenRegisterMoveCallback(
    _ callback: CGScreenUpdateMoveCallback,
    _ userInfo: UnsafeMutableRawPointer?
) -> CGError
```

Deprecated

Use display streaming instead. See Quartz Display Services.

## Parameters 

`callback`  

A pointer to the callback function to be registered.

`userInfo`  

A pointer to user-defined data, or `NULL`. The `userInfo` argument is passed back to the callback function each time it’s invoked.

## Return Value

A result code. See `Core Graphics Data Types and Constants`.

## Discussion

A callback function may be registered multiple times with different user-defined data pointers, resulting in multiple registration entries. For each registration, when notification is no longer needed, you should remove the registration by calling the function CGScreenUnregisterMoveCallback(_:_:).

The callback function you register is invoked only if your application has an active event loop. The callback is invoked in the same thread of execution that is processing events within your application.

### Special Considerations

This function is implemented in macOS 10.4.3 and later.

## See Also

### Functions

func CGAcquireDisplayFadeReservation(CGDisplayReservationInterval, UnsafeMutablePointer&lt;CGDisplayFadeReservationToken>?) -> CGError

Reserves the fade hardware for a specified time interval.

func CGAssociateMouseAndMouseCursorPosition(boolean_t) -> CGError

Connects or disconnects the mouse and cursor while an application is in the foreground.

func CGBeginDisplayConfiguration(UnsafeMutablePointer&lt;CGDisplayConfigRef?>?) -> CGError

Begins a new set of display configuration changes.

func CGCancelDisplayConfiguration(CGDisplayConfigRef?) -> CGError

Cancels a set of display configuration changes.

func CGCaptureAllDisplays() -> CGError

Obtains exclusive use of all active displays, preventing other applications and system services from using the display or changing its configuration.

func CGCaptureAllDisplaysWithOptions(CGCaptureOptions) -> CGError

Captures all attached displays, using the specified options.

func CGCompleteDisplayConfiguration(CGDisplayConfigRef?, CGConfigureOption) -> CGError

Completes a set of display configuration changes.

func CGConfigureDisplayFadeEffect(CGDisplayConfigRef?, CGDisplayFadeInterval, CGDisplayFadeInterval, Float, Float, Float) -> CGError

Modifies the settings of the built-in fade effect that occurs during a display configuration.

func CGConfigureDisplayMirrorOfDisplay(CGDisplayConfigRef?, CGDirectDisplayID, CGDirectDisplayID) -> CGError

Changes the configuration of a mirroring set.

func CGConfigureDisplayMode(CGDisplayConfigRef?, CGDirectDisplayID, CFDictionary?) -> CGError

Configures the display mode of a display.

Deprecated

func CGConfigureDisplayOrigin(CGDisplayConfigRef?, CGDirectDisplayID, Int32, Int32) -> CGError

Configures the origin of a display relative to the global display coordinate space.

func CGConfigureDisplayStereoOperation(CGDisplayConfigRef?, CGDirectDisplayID, boolean_t, boolean_t) -> CGError

Enables or disables stereo operation for a display, as part of a display configuration.

func CGConfigureDisplayWithDisplayMode(CGDisplayConfigRef?, CGDirectDisplayID, CGDisplayMode?, CFDictionary?) -> CGError

Configures the display mode of a display.

func CGCursorIsDrawnInFramebuffer() -> boolean_t

Returns a Boolean value indicating whether the mouse cursor is drawn in framebuffer memory.

Deprecated

func CGCursorIsVisible() -> boolean_t

Returns a Boolean value indicating whether the mouse cursor is visible.

Deprecated

