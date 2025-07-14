

- Core Graphics
- CGEventSource
-  getLocalEventsFilterDuringSuppressionState(\_:) 

Instance Method

# getLocalEventsFilterDuringSuppressionState(\_:)

Returns the mask that indicates which classes of local hardware events are enabled during event suppression.

Mac Catalyst 13.1+macOS 10.4+

``` source
func getLocalEventsFilterDuringSuppressionState(_ state: CGEventSuppressionState) -> CGEventFilterMask
```

## Parameters 

`state`  

The type of event suppression interval during which the filter is applied. Pass one of the constants listed in CGEventSuppressionState.

## Return Value

A mask that specifies the categories of local hardware events to enable during the event suppression interval. See CGEventFilterMask.

## Discussion

You can configure the system to suppress local hardware events from the keyboard or mouse during a short interval after a Quartz event is posted or during a synthetic mouse drag (mouse movement with the left or only mouse button down). For information about setting this local events filter, see setLocalEventsFilterDuringSuppressionState(_:state:).

This function lets you specify an event source and a suppression state (event suppression interval or mouse drag), and returns a filter mask of event categories to be passed through during suppression.

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

