

- Core Graphics
-  CGGetEventTapList(\_:\_:\_:) 

Function

# CGGetEventTapList(\_:\_:\_:)

Gets a list of currently installed event taps.

Mac Catalyst 13.1+macOS 10.4+

``` source
func CGGetEventTapList(
    _ maxNumberOfTaps: UInt32,
    _ tapList: UnsafeMutablePointer?,
    _ eventTapCount: UnsafeMutablePointer?
) -> CGError
```

## Parameters 

`maxNumberOfTaps`  

The length of the array you provide in the `tapList` parameter.

`tapList`  

An array of event tap information structures. You are responsible for allocating storage for the array. On return, your array contains a list of currently installed event taps. If you pass `NULL` in this parameter, the `maxNumberOfTaps` parameter is ignored, and the `eventTapCount` variable is filled in with the number of event taps that are currently installed.

`eventTapCount`  

A pointer to a `CGTableCount` variable. On return, the variable contains actual number of array elements filled in.

## Return Value

A result code. See the result codes described in Quartz Display Services.

## Discussion

Each call to this function has the side effect of resetting the minimum and maximum latency values in the `tapList` parameter to the corresponding average values. Values reported in these fields reflect the minimum and maximum values seen since the preceding call, or the instantiation of the tap. This allows a monitoring tool to evaluate the best and worst case latency over time and under various operating conditions.

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

