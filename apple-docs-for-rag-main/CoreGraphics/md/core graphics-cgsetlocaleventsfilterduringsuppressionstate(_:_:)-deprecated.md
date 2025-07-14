

- Core Graphics
-  CGSetLocalEventsFilterDuringSuppressionState(\_:\_:) Deprecated

Function

# CGSetLocalEventsFilterDuringSuppressionState(\_:\_:)

Filters local hardware events from the keyboard and mouse during the short interval after a synthetic event is posted.

Mac Catalyst 13.1–13.1Deprecated

``` source
func CGSetLocalEventsFilterDuringSuppressionState(
    _ filter: CGEventFilterMask,
    _ state: CGEventSuppressionState
) -> CGError
```

Deprecated

No longer supported

## Parameters 

`filter`  

The class of local hardware events to enable after a synthetic event is posted. Pass one of the constants listed in CGEventFilterMask.

`state`  

The type of interval during which the filter is applied. Pass one of the constants listed in CGEventSuppressionState.

## Return Value

A result code. See the result codes described in Quartz Display Services.

## Discussion

By default, the system suppresses local hardware events from the keyboard and mouse during a short interval after a synthetic event is posted and during a synthetic mouse drag (mouse movement with the left or only mouse button down).

Some applications may want to enable events from some of the local hardware. For example, if you post mouse events only, you may wish to permit local keyboard hardware events to pass through.

This function lets you specify a state (event suppression interval or mouse drag), and a mask of event categories to be passed through. The new filter state takes effect with the next synthetic event you post.

This function is not recommended for general use because of undocumented special cases and undesirable side effects. The recommended replacement for this function is setLocalEventsFilterDuringSuppressionState(_:state:), which allows the filter behavior to be associated only with events created from a specific event source.

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

