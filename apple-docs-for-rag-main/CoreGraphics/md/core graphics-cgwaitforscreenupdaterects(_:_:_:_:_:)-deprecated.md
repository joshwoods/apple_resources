

- Core Graphics
-  CGWaitForScreenUpdateRects(\_:\_:\_:\_:\_:) Deprecated

Function

# CGWaitForScreenUpdateRects(\_:\_:\_:\_:\_:)

Waits for screen update operations.

Mac Catalyst 13.1–13.1Deprecated

``` source
func CGWaitForScreenUpdateRects(
    _ requestedOperations: CGScreenUpdateOperation,
    _ currentOperation: UnsafeMutablePointer?,
    _ rects: UnsafeMutablePointer?>?,
    _ rectCount: UnsafeMutablePointer?,
    _ delta: UnsafeMutablePointer?
) -> CGError
```

Deprecated

Use display streaming instead. See Quartz Display Services.

## Parameters 

`requestedOperations`  

The desired types of screen update operations. There are several possible choices:

- Specify `kCGScreenUpdateOperationRefresh` if you want all move operations to be returned as refresh operations.

- Specify `(kCGScreenUpdateOperationRefresh | kCGScreenUpdateOperationMove)` if you want to distinguish between move and refresh operations.

- Add `kCGScreenUpdateOperationReducedDirtyRectangleCount` to the screen operations if you want to minimize the number of rectangles returned to represent changed areas of the display.

`currentOperation`  

A pointer to a `CGScreenUpdateOperation` variable. On return, the variable indicates the type of update operation (refresh or move).

`rects`  

A pointer to a `CGRect*` variable. On return, the variable contains an array of rectangles that bound the updated areas, specified in the global display coordinate space. When you no longer need the array, you should deallocate it by calling CGReleaseScreenRefreshRects(_:).

`rectCount`  

A pointer to a `size_t` variable. On return, the variable contains the number of entries in the returned array of rectangles.

`delta`  

A pointer to a `CGScreenUpdateMoveDelta` variable. On return, if the value of the `currentOperation` parameter is `kCGScreenUpdateOperationMove`, the variable contains the distance moved.

## Return Value

A result code. See `Core Graphics Data Types and Constants`.

## Discussion

In some applications it may be preferable to wait for screen-update data synchronously, using this function. You should call this function in a thread other than the main event-processing thread.

As an alternative, Quartz also supports asynchronous notification—see CGRegisterScreenRefreshCallback(_:_:) and CGScreenRegisterMoveCallback(_:_:). If refresh or move callback functions are registered, this function should not be used.

### Special Considerations

This function is implemented in macOS 10.4.3 and later.

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

