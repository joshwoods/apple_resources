

- Core Graphics
-  CGConfigureDisplayWithDisplayMode(\_:\_:\_:\_:) 

Function

# CGConfigureDisplayWithDisplayMode(\_:\_:\_:\_:)

Configures the display mode of a display.

Mac Catalyst 13.1+macOS 10.6+

``` source
func CGConfigureDisplayWithDisplayMode(
    _ config: CGDisplayConfigRef?,
    _ display: CGDirectDisplayID,
    _ mode: CGDisplayMode?,
    _ options: CFDictionary?
) -> CGError
```

## Parameters 

`config`  

A display configuration you aquire by calling CGBeginDisplayConfiguration(_:).

`display`  

The identifier of the display to configure.

`mode`  

A display mode to configure.

`options`  

Reserved for future expansion. Pass `NULL` for now.

## Return Value

A result code. If the request to change modes is successful, the result is `kCGErrorSuccess`. For other possible values, see CGError.

## Discussion

This function allows you to specify a display mode with which to configure the display using a transaction. Before using this function, call CGBeginDisplayConfiguration(_:) to acquire the display configuration token for the desired display. Call CGCompleteDisplayConfiguration(_:_:) to execute the transaction.

Using this function to change the mode of a display in a mirroring set might cause Quartz to adjust settings of the other displays in the set. When necessary, Quartz adjusts the bounds, resolutions, and depth of the displays to a safe mode with matching depth and the smallest enclosing size.

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

func CGCursorIsDrawnInFramebuffer() -> boolean_t

Returns a Boolean value indicating whether the mouse cursor is drawn in framebuffer memory.

Deprecated

func CGCursorIsVisible() -> boolean_t

Returns a Boolean value indicating whether the mouse cursor is visible.

Deprecated

func CGDirectDisplayCopyCurrentMetalDevice(CGDirectDisplayID) -> (any MTLDevice)?

Returns the GPU device instance that’s currently driving a display.

