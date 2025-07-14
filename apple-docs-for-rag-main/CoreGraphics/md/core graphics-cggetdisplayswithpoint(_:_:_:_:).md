

- Core Graphics
-  CGGetDisplaysWithPoint(\_:\_:\_:\_:) 

Function

# CGGetDisplaysWithPoint(\_:\_:\_:\_:)

Provides a list of online displays with bounds that include the specified point.

Mac Catalyst 13.1+macOS 10.0+

``` source
func CGGetDisplaysWithPoint(
    _ point: CGPoint,
    _ maxDisplays: UInt32,
    _ displays: UnsafeMutablePointer?,
    _ matchingDisplayCount: UnsafeMutablePointer?
) -> CGError
```

## Parameters 

`point`  

The coordinates of a point in the global display coordinate space. The origin is the upper-left corner of the main display.

`maxDisplays`  

The size of the `displays` array. This value determines the maximum number of displays the list includes.

`displays`  

A pointer to storage you provide for an array of display IDs. On return, the array contains a list of displays with bounds that include the point. If you pass `NULL`, on return the display count contains the total number of displays with bounds that include the point.

`matchingDisplayCount`  

A pointer to a display count variable you provide. On return, the display count contains the actual number of displays the list includes in the `dspys` array. This value is at most `maxDisplays`.

## Return Value

A result code. To interpret the result code, see CGError.

## Discussion

If the `displays` array is `nil`, this function ignores the `maxDisplays` parameter. If the `maxDisplays` parameter is `0`, this function ignores the `displays` array. In any case, this function fills in the `matchingDisplayCount` pointer with the number of displays that contain the specified point.

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

