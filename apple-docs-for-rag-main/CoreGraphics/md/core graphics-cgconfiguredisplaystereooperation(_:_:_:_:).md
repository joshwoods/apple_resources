

- Core Graphics
-  CGConfigureDisplayStereoOperation(\_:\_:\_:\_:) 

Function

# CGConfigureDisplayStereoOperation(\_:\_:\_:\_:)

Enables or disables stereo operation for a display, as part of a display configuration.

Mac Catalyst 13.1+macOS 10.4+

``` source
func CGConfigureDisplayStereoOperation(
    _ config: CGDisplayConfigRef?,
    _ display: CGDirectDisplayID,
    _ stereo: boolean_t,
    _ forceBlueLine: boolean_t
) -> CGError
```

## Parameters 

`config`  

A display configuration, acquired by calling CGBeginDisplayConfiguration(_:).

`display`  

The identifier of the display being configured.

`stereo`  

Pass `true` if you want to enable stereo operation. To disable it, pass `false`.

`forceBlueLine`  

When in stereo operation, a display may need to generate a special stereo sync signal as part of the video output. The sync signal consists of a blue line which occupies the first 25% of the last scan line for the left eye view, and the first 75% of the last scan line for the right eye view. The remainder of the scan line is black. To force the display to generate this sync signal, pass `true`; otherwise, pass `false`.

## Return Value

A result code. See `Core Graphics Data Types and Constants`.

## Discussion

The system normally detects the presence of a stereo window and automatically switches a display containing a stereo window to stereo operation. This function provides a mechanism to force a display to stereo operation, and to set options (blue line sync signal) when in stereo operation.

On success, the display resolution, mirroring mode, and available display modes may change due to hardware-specific capabilities and limitations. You should check these settings to verify that they are appropriate for your application.

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

func CGConfigureDisplayWithDisplayMode(CGDisplayConfigRef?, CGDirectDisplayID, CGDisplayMode?, CFDictionary?) -> CGError

Configures the display mode of a display.

func CGCursorIsDrawnInFramebuffer() -> boolean_t

Returns a Boolean value indicating whether the mouse cursor is drawn in framebuffer memory.

Deprecated

func CGCursorIsVisible() -> boolean_t

Returns a Boolean value indicating whether the mouse cursor is visible.

Deprecated

func CGDirectDisplayCopyCurrentMetalDevice(CGDirectDisplayID) -> (any MTLDevice)?

Returns the GPU device instance that’s currently driving a display.

