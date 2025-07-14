

- Core Graphics
-  CGConfigureDisplayOrigin(\_:\_:\_:\_:) 

Function

# CGConfigureDisplayOrigin(\_:\_:\_:\_:)

Configures the origin of a display relative to the global display coordinate space.

Mac Catalyst 13.1+macOS 10.0+

``` source
func CGConfigureDisplayOrigin(
    _ config: CGDisplayConfigRef?,
    _ display: CGDirectDisplayID,
    _ x: Int32,
    _ y: Int32
) -> CGError
```

## Parameters 

`config`  

A display configuration that you acquire by calling CGBeginDisplayConfiguration(_:).

`display`  

The identifier of the display to configure.

`x`  

The desired x-coordinate for the upper-left corner of the display.

`y`  

The desired y-coordinate for the upper-left corner of the display.

## Return Value

A result code. If the request to configure the origin of the display is successful, the result is `kCGErrorSuccess`. For other possible values, see CGError.

## Discussion

In Quartz, the upper-left corner of a display is the origin. You specify the origin of a display in the global display coordinate space. The origin of the main or primary display is `(0,0)`.

The placement of the new origin is as close as possible to the requested location, without overlapping or leaving a gap between displays.

If you use this function to change the origin of a mirrored display, the mirrored set might not include the display.

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

func CGDirectDisplayCopyCurrentMetalDevice(CGDirectDisplayID) -> (any MTLDevice)?

Returns the GPU device instance that’s currently driving a display.

