

- Core Graphics
-  CGGetDisplayTransferByFormula(\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:) 

Function

# CGGetDisplayTransferByFormula(\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:)

Gets the coefficients of the gamma transfer formula for a display.

Mac Catalyst 13.1+macOS 10.0+

``` source
func CGGetDisplayTransferByFormula(
    _ display: CGDirectDisplayID,
    _ redMin: UnsafeMutablePointer?,
    _ redMax: UnsafeMutablePointer?,
    _ redGamma: UnsafeMutablePointer?,
    _ greenMin: UnsafeMutablePointer?,
    _ greenMax: UnsafeMutablePointer?,
    _ greenGamma: UnsafeMutablePointer?,
    _ blueMin: UnsafeMutablePointer?,
    _ blueMax: UnsafeMutablePointer?,
    _ blueGamma: UnsafeMutablePointer?
) -> CGError
```

## Parameters 

`display`  

The identifier of the display to access.

`redMin`  

The minimum value of the red channel in the gamma table. The value is a number in the interval `[0, redMax]`.

`redMax`  

The maximum value of the red channel in the gamma table. The value is a number in the interval `[redMin, 1]`.

`redGamma`  

A positive value used to compute the red channel in the gamma table.

`greenMin`  

The minimum value of the green channel in the gamma table. The value is a number in the interval `[0, greenMax]`.

`greenMax`  

The maximum value of the green channel in the gamma table. The value is a number in the interval `[greenMin, 1]`.

`greenGamma`  

A positive value used to compute the green channel in the gamma table.

`blueMin`  

The minimum value of the blue channel in the gamma table. The value is a number in the interval `[0, blueMax]`.

`blueMax`  

The maximum value of the blue channel in the gamma table. The value is a number in the interval `[blueMin, 1]`.

`blueGamma`  

A positive value used to compute the blue channel in the gamma table.

## Return Value

A result code. To interpret the result code, see CGError.

## Discussion

For information about the gamma transfer formula, see the description of the function CGSetDisplayTransferByFormula(_:_:_:_:_:_:_:_:_:_:).

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

