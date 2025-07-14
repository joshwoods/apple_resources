

- Core Graphics
-  CGConfigureDisplayMirrorOfDisplay(\_:\_:\_:) 

Function

# CGConfigureDisplayMirrorOfDisplay(\_:\_:\_:)

Changes the configuration of a mirroring set.

Mac Catalyst 13.1+macOS 10.2+

``` source
func CGConfigureDisplayMirrorOfDisplay(
    _ config: CGDisplayConfigRef?,
    _ display: CGDirectDisplayID,
    _ master: CGDirectDisplayID
) -> CGError
```

## Parameters 

`config`  

A display configuration, acquired by calling CGBeginDisplayConfiguration(_:).

`display`  

The identifier of the display to add to a mirroring set.

`master`  

A display in a mirroring set, or `kCGNullDirectDisplay` to disable mirroring. To specify the main display, use CGMainDisplayID().

## Return Value

A result code. See `Core Graphics Data Types and Constants`.

## Discussion

Display mirroring and display matte generation are implemented either in hardware (preferred) or software, at the discretion of the device driver.

- Hardware mirroring

With hardware mirroring enabled, all drawing is directed to the primary display—see CGDisplayPrimaryDisplay(_:).

If the device driver selects hardware matte generation, the display bounds and row-bytes values are adjusted to reflect the active drawable area.

- Software mirroring

In this form of mirroring, identical content is drawn into each display in the mirroring set. Applications that use the window system need not be concerned about mirroring, as the window system takes care of all flushing of window content to the appropriate displays.

Applications that draw directly to the display, as with display capture, must make sure to draw the same content to all mirrored displays in a software mirror set. When drawing to software mirrored displays using a full screen OpenGL context (not drawing through a window), you should create shared OpenGL contexts for each display and rerender for each display.

You can use the function CGGetActiveDisplayList(_:_:_:) to determine which displays are active, or drawable. This automatically gives your application the correct view of the current displays.

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

