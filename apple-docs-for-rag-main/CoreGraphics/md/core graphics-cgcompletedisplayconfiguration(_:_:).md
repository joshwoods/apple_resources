

- Core Graphics
-  CGCompleteDisplayConfiguration(\_:\_:) 

Function

# CGCompleteDisplayConfiguration(\_:\_:)

Completes a set of display configuration changes.

Mac Catalyst 13.1+macOS 10.0+

``` source
func CGCompleteDisplayConfiguration(
    _ config: CGDisplayConfigRef?,
    _ option: CGConfigureOption
) -> CGError
```

## Parameters 

`config`  

The display configuration that contains the desired changes. On return, this configuration is no longer valid.

`option`  

The scope of the display configuration changes. Pass one of the constants listed in CGConfigureOption.

## Return Value

A result code. If the request to apply changes is successful, the result is `kCGErrorSuccess`. For other possible values, see CGError.

## Discussion

This function applies a set of display configuration changes as a single atomic transaction. The duration or scope of the changes depends on the value of the `option` parameter. For more information about possible scopes, see CGConfigureOption.

A configuration change can fail if you request an unsupported display mode or if another application is running in full-screen mode.

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

func CGDirectDisplayCopyCurrentMetalDevice(CGDirectDisplayID) -> (any MTLDevice)?

Returns the GPU device instance that’s currently driving a display.

