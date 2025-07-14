

- Core Graphics
-  CGInhibitLocalEvents(\_:) Deprecated

Function

# CGInhibitLocalEvents(\_:)

Turns off local hardware events in the current session.

Mac Catalyst 13.1–13.1Deprecated

``` source
func CGInhibitLocalEvents(_ inhibit: boolean_t) -> CGError
```

Deprecated

No longer supported

## Parameters 

`inhibit`  

Pass `true` to specify that local hardware events on the remote system should be inhibited; otherwise, pass `false`.

## Return Value

A result code. See the result codes described in Quartz Display Services.

## Discussion

This function is typically used during remote operation of a system to disconnect the keyboard and mouse for a short period of time, as in automated system testing or telecommuting applications.

The `CGInhibitLocalEvents` function is not recommended for general use because of undocumented special cases and undesirable side effects. For example, this function can permanently disable the keyboard and mouse, rendering the system unusable. The recommended replacement for this function is setLocalEventsFilterDuringSuppressionState(_:state:).

### Special Considerations

In OS X v10.2 and earlier, this function inhibits local events only after a synthetic keyboard or mouse event is posted by the calling application. In macOS 10.3 and later, event inhibition takes effect immediately. If your application terminates for any reason, event inhibition on the remote system is immediately turned off.

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

