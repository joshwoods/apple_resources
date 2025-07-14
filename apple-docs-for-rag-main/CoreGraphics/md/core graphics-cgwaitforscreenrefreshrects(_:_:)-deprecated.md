

- Core Graphics
-  CGWaitForScreenRefreshRects(\_:\_:) Deprecated

Function

# CGWaitForScreenRefreshRects(\_:\_:)

Waits for screen refresh operations.

Mac Catalyst 13.1–13.1Deprecated

``` source
func CGWaitForScreenRefreshRects(
    _ rects: UnsafeMutablePointer?>?,
    _ count: UnsafeMutablePointer?
) -> CGError
```

Deprecated

Use display streaming instead. See Quartz Display Services.

## Parameters 

`rects`  

A pointer to a `CGRect*` variable. On return, the variable contains an array of rectangles that bound the refreshed areas, specified in the global display coordinate space. When you no longer need the array, you should deallocate it by calling CGReleaseScreenRefreshRects(_:).

`count`  

A pointer to a `CGRectCount` variable. On return, the variable contains the number of entries in the returned array of rectangles.

## Return Value

A result code. See `Core Graphics Data Types and Constants`.

## Discussion

In some applications it may be preferable to wait for screen-refresh data synchronously, using this function. You should call this function in a thread other than the main event-processing thread.

As an alternative, Quartz also supports asynchronous notification—see CGRegisterScreenRefreshCallback(_:_:). If refresh callback functions are registered, this function should not be used.

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

