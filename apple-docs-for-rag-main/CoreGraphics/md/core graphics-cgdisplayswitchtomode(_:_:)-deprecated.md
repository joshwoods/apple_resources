

- Core Graphics
-  CGDisplaySwitchToMode(\_:\_:) Deprecated

Function

# CGDisplaySwitchToMode(\_:\_:)

Switches a display to a different mode.

Mac Catalyst 13.1–13.1Deprecated

``` source
func CGDisplaySwitchToMode(
    _ display: CGDirectDisplayID,
    _ mode: CFDictionary?
) -> CGError
```

Deprecated

Use CGDisplaySetDisplayMode(_:_:_:) instead.

## Parameters 

`display`  

The identifier of the display to be accessed.

`mode`  

A display mode dictionary that contains information about the display mode to set. The dictionary passed in must be a dictionary returned by another Quartz display function such as CGDisplayAvailableModes(_:) or CGDisplayBestModeForParameters(_:_:_:_:_:). For a list of the properties in a display mode dictionary, see Display Mode Standard Properties and Display Mode Optional Properties. For general information about using dictionaries, see CFDictionary.

## Return Value

A result code. See `Core Graphics Data Types and Constants`.

## Discussion

This function switches the display mode of the specified display. The operation is always synchronous; the function does not return until the mode switch is complete. Note that after switching, display parameters and addresses may change.

The selected display mode persists for the life of the calling program. When the program terminates, the display mode automatically reverts to the permanent setting in the Displays panel of System Preferences.

When changing the display mode of a display in a mirroring set, other displays in the mirroring set will be assigned a mode that’s capable of mirroring the bounds of the display being adjusted. To avoid this automatic behavior, you can use the following procedure: callCGBeginDisplayConfiguration(_:), call CGConfigureDisplayMode(_:_:_:) for each display to explicitly set the mode, and finally call CGCompleteDisplayConfiguration(_:_:)

### Special Considerations

This deprecated function takes as a parameter a display mode dictionary. Starting in OS X v10.6, display mode dictionaries have been replaced by the `CGDisplayMode` opaque type.

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

