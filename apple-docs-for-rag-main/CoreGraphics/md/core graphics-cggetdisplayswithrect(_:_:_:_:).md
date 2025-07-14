

- Core Graphics
-  CGGetDisplaysWithRect(\_:\_:\_:\_:) 

Function

# CGGetDisplaysWithRect(\_:\_:\_:\_:)

Gets a list of online displays with bounds that intersect the specified rectangle.

Mac Catalyst 13.1+macOS 10.0+

``` source
func CGGetDisplaysWithRect(
    _ rect: CGRect,
    _ maxDisplays: UInt32,
    _ displays: UnsafeMutablePointer?,
    _ matchingDisplayCount: UnsafeMutablePointer?
) -> CGError
```

## Parameters 

`rect`  

The location and size of a rectangle in the global display coordinate space. The origin is the upper-left corner of the main display.

`maxDisplays`  

The size of the `displays` array. This value determines the maximum number of displays that can be returned in the `displays` parameter. Generally, you should specify a number greater than 0 for this parameter. If you specify 0, the value returned in `matchingDisplayCount` is undefined and this function sets the `displays` parameter to `NULL`.

`displays`  

A pointer to storage provided by the caller for an array of display IDs. On return, the array contains a list of displays whose bounds intersect the specified rectangle.

`matchingDisplayCount`  

A pointer to a display count variable provided by the caller. On return, this variable contains the number of displays that were returned in the `displays` parameter. You must provide a non-`NULL` value for this parameter.

## Return Value

A result code. See `Core Graphics Data Types and Constants`.

## Discussion

If the `dspys` array is `NULL`, this function ignores the `maxDisplays` parameter. If the `maxDisplays` parameter is `0`, this function ignores the `displays` array. In any case, this function fills in the `matchingDisplayCount` pointer with the number of displays that intersect the specified rectangle.

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

