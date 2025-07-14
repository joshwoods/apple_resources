

- Core Graphics
-  CGGetActiveDisplayList(\_:\_:\_:) 

Function

# CGGetActiveDisplayList(\_:\_:\_:)

Provides a list of displays that are active for drawing.

Mac Catalyst 13.1+macOS 10.0+

``` source
func CGGetActiveDisplayList(
    _ maxDisplays: UInt32,
    _ activeDisplays: UnsafeMutablePointer?,
    _ displayCount: UnsafeMutablePointer?
) -> CGError
```

## Parameters 

`maxDisplays`  

The size of the `activeDisplays` array. This value determines the maximum number of displays the list includes.

`activeDisplays`  

A pointer to storage you provide for an array of display IDs. On return, the array contains a list of active displays. If you pass `NULL`, on return the display count contains the total number of active displays.

`displayCount`  

A pointer to a display count variable you provide. On return, the display count contains the actual number of displays the function added to the `activeDisplays` array. This value is at most `maxDisplays`.

## Return Value

A result code. To interpret the result code, see CGError.

## Discussion

The first entry in the list of active displays is the main display. In case of mirroring, the first entry is the largest drawable display or, if all are the same size, the display with the greatest pixel depth.

Note that when using hardware mirroring between displays, only the primary display is active and appears in the list. When using software mirroring, all the mirrored displays are active and appear in the list. For more information about mirroring, see CGConfigureDisplayMirrorOfDisplay(_:_:_:).

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

