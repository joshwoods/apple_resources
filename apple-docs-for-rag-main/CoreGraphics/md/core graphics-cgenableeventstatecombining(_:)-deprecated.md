

- Core Graphics
-  CGEnableEventStateCombining(\_:) Deprecated

Function

# CGEnableEventStateCombining(\_:)

Enables or disables the merging of actual key and mouse state with the application-specified state in a synthetic event.

Mac Catalyst 13.1–13.1Deprecated

``` source
func CGEnableEventStateCombining(_ combineState: boolean_t) -> CGError
```

Deprecated

No longer supported

## Parameters 

`combineState`  

Pass `true` to specify that the actual key and mouse state are merged with the application-specified state in a synthetic event; otherwise, pass `false`.

## Return Value

A result code. See the result codes described in Quartz Display Services.

## Discussion

By default, the flags that indicate modifier key state (Command, Option, Shift, Control, and so on) from the system’s keyboard and from other event sources are ORed together as an event is posted into the system, and current key and mouse button state is considered in generating new events. This function allows your application to enable or disable the merging of event state. When combining is turned off, the event state propagated in the events posted by your application reflect state built up only by your application. The state within your application’s generated event will not be combined with the system’s current state, so the system-wide state reflecting key and mouse button state will remain unchanged. When called with `doCombineState` equal to `false`, this function initializes local (per application) state tracking information to a state of all keys, modifiers, and mouse buttons up. When called with `doCombineState` equal to `true`, the current global state of keys, modifiers, and mouse buttons are used in generating events.

This function is not recommended for general use because of undocumented special cases and undesirable side effects. The recommended replacement for this function is to use Quartz events and Quartz event sources. This allows you to control exactly which, if any, external event sources will contribute to the state used to create an event.

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

