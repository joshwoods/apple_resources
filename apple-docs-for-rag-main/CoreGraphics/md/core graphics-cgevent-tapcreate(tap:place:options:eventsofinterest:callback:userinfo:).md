

- Core Graphics
- CGEvent
-  tapCreate(tap:place:options:eventsOfInterest:callback:userInfo:) 

Type Method

# tapCreate(tap:place:options:eventsOfInterest:callback:userInfo:)

Creates an event tap.

Mac Catalyst 13.1+macOS 10.4+

``` source
class func tapCreate(
    tap: CGEventTapLocation,
    place: CGEventTapPlacement,
    options: CGEventTapOptions,
    eventsOfInterest: CGEventMask,
    callback: CGEventTapCallBack,
    userInfo: UnsafeMutableRawPointer?
) -> CFMachPort?
```

## Parameters 

`tap`  

The location of the new event tap. Pass one of the constants listed in CGEventTapLocation. Only processes running as the root user may locate an event tap at the point where HID events enter the window server; for other users, this function returns `NULL`.

`place`  

The placement of the new event tap in the list of active event taps. Pass one of the constants listed in CGEventTapPlacement.

`options`  

A constant that specifies whether the new event tap is a passive listener or an active filter.

`eventsOfInterest`  

A bit mask that specifies the set of events to be observed. For a list of possible events, see CGEventType. For information on how to specify the mask, see CGEventMask. If the event tap is not permitted to monitor one or more of the events specified in the `eventsOfInterest` parameter, then the appropriate bits in the mask are cleared. If that action results in an empty mask, this function returns `NULL`.

`callback`  

An event tap callback function that you provide. Your callback function is invoked from the run loop to which the event tap is added as a source. The thread safety of the callback is defined by the run loop’s environment. To learn more about event tap callbacks, see CGEventTapCallBack.

`userInfo`  

A pointer to user-defined data. This pointer is passed into the callback function specified in the `callback` parameter.

## Return Value

A Core Foundation mach port that represents the new event tap, or `NULL` if the event tap could not be created. When you are finished using the event tap, you should release the mach port using the function `CFRelease`. Releasing the mach port also releases the tap.

## Discussion

Event taps receive key up and key down events if one of the following conditions is true:

- The current process is running as the root user.

- Access for assistive devices is enabled. In OS X v10.4, you can enable this feature using System Preferences, Universal Access panel, Keyboard view.

After creating an event tap, you can add it to a run loop as follows:

1.  Pass the event tap to the CFMachPortCreateRunLoopSource(_:_:_:) function to create a run loop event source.

2.  Call the CFRunLoopAddSource(_:_:_:) function to add the source to the appropriate run loop.

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

