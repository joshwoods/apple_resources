

- Core Graphics
-  CGConfigureDisplayMode(\_:\_:\_:) Deprecated

Function

# CGConfigureDisplayMode(\_:\_:\_:)

Configures the display mode of a display.

Mac Catalyst 13.1–13.1Deprecated

``` source
func CGConfigureDisplayMode(
    _ config: CGDisplayConfigRef?,
    _ display: CGDirectDisplayID,
    _ mode: CFDictionary?
) -> CGError
```

Deprecated

Use CGConfigureDisplayWithDisplayMode(_:_:_:_:) instead.

## Parameters 

`config`  

A display configuration, acquired by calling CGBeginDisplayConfiguration(_:).

`display`  

The identifier of the display being configured.

`mode`  

A display mode dictionary (see the discussion below).

## Return Value

A result code. See `Core Graphics Data Types and Constants`.

## Discussion

A display mode is a set of properties such as width, height, pixel depth, and refresh rate, and options such as stretched LCD panel filling.

The display mode you provide must be one of the following:

- A dictionary returned by one of the `CGDisplayBestMode` functions, such as CGDisplayBestModeForParameters(_:_:_:_:_:).

- A dictionary in the array returned by CGDisplayAvailableModes(_:).

If you use this function to change the mode of a display in a mirroring set, Quartz may adjust the bounds, resolutions, and depth of the other displays in the set to a safe mode, with matching depth and the smallest enclosing size.

### Special Considerations

This deprecated function takes as a parameter a display mode dictionary. Starting in OS X v10.6, display mode dictionaries have been replaced by the `CGDisplayMode` opaque type. For information on the `CGDisplayMode` opaque type, see Getting Information About a Display Mode.

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

func CGDirectDisplayCopyCurrentMetalDevice(CGDirectDisplayID) -> (any MTLDevice)?

Returns the GPU device instance that’s currently driving a display.

