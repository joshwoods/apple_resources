

- Core Graphics
-  CGDisplayBestModeForParameters(\_:\_:\_:\_:\_:) Deprecated

Function

# CGDisplayBestModeForParameters(\_:\_:\_:\_:\_:)

Returns information about the display mode closest to a specified depth and screen size.

Mac Catalyst 13.1–13.1Deprecated

``` source
func CGDisplayBestModeForParameters(
    _ display: CGDirectDisplayID,
    _ bitsPerPixel: Int,
    _ width: Int,
    _ height: Int,
    _ exactMatch: UnsafeMutablePointer?
) -> CFDictionary?
```

Deprecated

Use the display mode query functions instead; see Getting Information About a Display Mode.

## Parameters 

`display`  

The identifier of the display to optimize.

`bitsPerPixel`  

Optimal display depth in bits per pixel. Note that this value is not the same as pixel depth, which is the number of bits per channel or component.

`width`  

Optimal display width in pixel units.

`height`  

Optimal display height in pixel units.

`exactMatch`  

A pointer to a Boolean variable. On return, its value is `true` if an exact match in display depth, width, and height is found; otherwise, `false`. If this information is not needed, pass `NULL`.

## Return Value

A display mode dictionary, or `NULL` if the display is invalid. The dictionary is owned by the system and you should not release it. The dictionary contains information about the display mode closest to the specified depth and screen size. For a list of the properties in a display mode dictionary, see Display Mode Standard Properties and Display Mode Optional Properties. For general information about using dictionaries, see CFDictionary.

## Discussion

This function tries to find an optimal display mode for the specified display. The function first tries to find a mode with the specified pixel depth and dimensions equal to or greater than the specified width and height. If no depth match is found, it tries to find a mode with greater depth and the same or greater dimensions. If a suitable display mode is not found, this function simply returns the current display mode.

### Special Considerations

This deprecated function selects a display mode closest to the specified parameters. Starting in OS X v10.6 new display mode APIs should be used to query display modes so that an application can tailor its definition of “best” to its graphics and memory needs.

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

