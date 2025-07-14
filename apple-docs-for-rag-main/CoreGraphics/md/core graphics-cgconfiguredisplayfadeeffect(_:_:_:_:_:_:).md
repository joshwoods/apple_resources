

- Core Graphics
-  CGConfigureDisplayFadeEffect(\_:\_:\_:\_:\_:\_:) 

Function

# CGConfigureDisplayFadeEffect(\_:\_:\_:\_:\_:\_:)

Modifies the settings of the built-in fade effect that occurs during a display configuration.

Mac Catalyst 13.1+macOS 10.2+

``` source
func CGConfigureDisplayFadeEffect(
    _ config: CGDisplayConfigRef?,
    _ fadeOutSeconds: CGDisplayFadeInterval,
    _ fadeInSeconds: CGDisplayFadeInterval,
    _ fadeRed: Float,
    _ fadeGreen: Float,
    _ fadeBlue: Float
) -> CGError
```

## Parameters 

`config`  

A display configuration, acquired by calling CGBeginDisplayConfiguration(_:).

`fadeOutSeconds`  

The time, in seconds, to fade from the normal display to the specified fade color. The fade out is completed before the display configuration is changed. If the interval is 0, Quartz applies the color immediately.

`fadeInSeconds`  

The time, in seconds, to return from the specified fade color to the normal display. The fade-in is run asynchronously after the display configuration is changed.

`fadeRed`  

An intensity value in the interval \[0, 1\] that represents the red component of the desired blend color.

`fadeGreen`  

An intensity value in the interval \[0, 1\] that represents the green component of the desired blend color.

`fadeBlue`  

An intensity value in the interval \[0, 1\] that represents the blue component of the desired blend color.

## Return Value

A result code. See `Core Graphics Data Types and Constants`.

## Discussion

This function provides a way to customize the built-in fade effect that Quartz performs when displays are reconfigured. The default time settings for this fade effect are 0.3 seconds to fade out, and 0.5 seconds to fade back in. The default fade color is French Blue for a normal desktop, and black for a captured display.

Before using this function, you need to call CGBeginDisplayConfiguration(_:) to acquire the display configuration token for the desired display. No fade reservation is needed—when you call CGCompleteDisplayConfiguration(_:_:), Quartz reserves the fade hardware (assuming it is available) and performs the fade.

Calling this function modifies the fade behavior for a single display configuration and has no permanent effect.

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

