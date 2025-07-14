

- Core Graphics
- CGEvent
-  tapCreateForPSN(processSerialNumber:place:options:eventsOfInterest:callback:userInfo:) 

Type Method

# tapCreateForPSN(processSerialNumber:place:options:eventsOfInterest:callback:userInfo:)

Creates an event tap for a specified process.

Mac Catalyst 13.1+macOS 10.4+

``` source
class func tapCreateForPSN(
    processSerialNumber: UnsafeMutableRawPointer,
    place: CGEventTapPlacement,
    options: CGEventTapOptions,
    eventsOfInterest: CGEventMask,
    callback: CGEventTapCallBack,
    userInfo: UnsafeMutableRawPointer?
) -> CFMachPort?
```

## Parameters 

`processSerialNumber`  

The process to monitor.

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

This function creates an event tap that receives events being routed by the window server to the specified process. For more information about creating event taps, see tapCreate(tap:place:options:eventsOfInterest:callback:userInfo:).

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

