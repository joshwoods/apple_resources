

- Core Graphics
-  CGGetDisplayTransferByTable(\_:\_:\_:\_:\_:\_:) 

Function

# CGGetDisplayTransferByTable(\_:\_:\_:\_:\_:\_:)

Gets the values in the RGB gamma tables for a display.

Mac Catalyst 13.1+macOS 10.0+

``` source
func CGGetDisplayTransferByTable(
    _ display: CGDirectDisplayID,
    _ capacity: UInt32,
    _ redTable: UnsafeMutablePointer?,
    _ greenTable: UnsafeMutablePointer?,
    _ blueTable: UnsafeMutablePointer?,
    _ sampleCount: UnsafeMutablePointer?
) -> CGError
```

## Parameters 

`display`  

The identifier of the display to be accessed.

`capacity`  

The number of entries each table can hold.

`redTable`  

A pointer to an array of type `CGGammaValue` with size `capacity`. On return, the array contains the values of the red channel in the display’s gamma table.

`greenTable`  

A pointer to an array of type `CGGammaValue` with size `capacity`. On return, the array contains the values of the green channel in the display’s gamma table.

`blueTable`  

A pointer to an array of type `CGGammaValue` with size `capacity`. On return, the array contains the values of the blue channel in the display’s gamma table.

`sampleCount`  

The number of samples actually copied into each array.

## Return Value

A result code. See `Core Graphics Data Types and Constants`.

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

