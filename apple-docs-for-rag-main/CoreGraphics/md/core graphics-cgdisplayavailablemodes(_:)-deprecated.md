

- Core Graphics
-  CGDisplayAvailableModes(\_:) Deprecated

Function

# CGDisplayAvailableModes(\_:)

Returns information about the currently available display modes.

Mac Catalyst 13.1–13.1Deprecated

``` source
func CGDisplayAvailableModes(_ dsp: CGDirectDisplayID) -> CFArray?
```

Deprecated

Use CGDisplayCopyAllDisplayModes(_:_:) instead.

## Parameters 

`dsp`  

The identifier of the display to be accessed.

## Return Value

An array of dictionaries with display mode information, or `NULL` if the display is invalid. The array is owned by the system and you should not release it. Each dictionary in the array contains information about a mode that the display supports. For a list of the properties in a display mode dictionary, see Display Mode Standard Properties and Display Mode Optional Properties. For general information about using dictionaries, see CFDictionary.

## Discussion

This deprecated function returns an array of display mode dictionary. Starting in OS X v10.6, display mode dictionaries have been replaced by the `CGDisplayMode` opaque type. Whereas display mode dictionaries returned by `CGDisplayAvailableModes` are owned by the system and are not to be released, display mode opaque type references returned by `CGDisplayCopyAllDisplayModes` are owned by the caller and you must release them.

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

