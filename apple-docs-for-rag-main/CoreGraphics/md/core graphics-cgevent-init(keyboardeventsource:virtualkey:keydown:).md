

- Core Graphics
- CGEvent
-  init(keyboardEventSource:virtualKey:keyDown:) 

Initializer

# init(keyboardEventSource:virtualKey:keyDown:)

Returns a new Quartz keyboard event.

Mac Catalyst 13.1+macOS 10.4+

``` source
init?(
    keyboardEventSource source: CGEventSource?,
    virtualKey: CGKeyCode,
    keyDown: Bool
)
```

## Parameters 

`source`  

An event source taken from another event, or `NULL`.

`virtualKey`  

The virtual key code for the event.

`keyDown`  

Pass `true` to specify that the key position is down. To specify that the key position is up, pass `false`. This value is used to determine the type of the keyboard event—see CGEventType.

## Return Value

A new keyboard event, or `NULL` if the event could not be created. When you no longer need the event, you should release it using the function `CFRelease`.

## Discussion

All keystrokes needed to generate a character must be entered, including modifier keys. For example, to produce a ‘Z’, the SHIFT key must be down, the ‘z’ key must go down, and then the SHIFT and ‘z’ key must be released:

```
CGEventRef event1, event2, event3, event4;
event1 = CGEventCreateKeyboardEvent (NULL, (CGKeyCode)56, true);
event2 = CGEventCreateKeyboardEvent (NULL, (CGKeyCode)6, true);
event3 = CGEventCreateKeyboardEvent (NULL, (CGKeyCode)6, false);
event4 = CGEventCreateKeyboardEvent (NULL, (CGKeyCode)56, false);
```

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

