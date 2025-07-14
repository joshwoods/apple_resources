

- Core Graphics
-  CGGetOnlineDisplayList(\_:\_:\_:) 

Function

# CGGetOnlineDisplayList(\_:\_:\_:)

Provides a list of displays that are online (active, mirrored, or sleeping).

Mac Catalyst 13.1+macOS 10.2+

``` source
func CGGetOnlineDisplayList(
    _ maxDisplays: UInt32,
    _ onlineDisplays: UnsafeMutablePointer?,
    _ displayCount: UnsafeMutablePointer?
) -> CGError
```

## Parameters 

`maxDisplays`  

The size of the `onlineDisplays` array. This value determines the maximum number of display IDs that can be returned.

`onlineDisplays`  

A pointer to storage provided by the caller for an array of display IDs. On return, the array contains a list of the online displays. If you pass `NULL`, on return the display count contains the total number of online displays.

`displayCount`  

A pointer to a display count variable provided by the caller. On return, the display count contains the actual number of displays returned in the `onlineDisplays` array. This value is at most `maxDisplays`.

## Return Value

A result code. See `Core Graphics Data Types and Constants`.

## Discussion

If the framebuffer hardware is connected, a display is considered connected or online.

When hardware mirroring is used, a display can be online but not active or drawable. Programs that manipulate display settings (such as gamma tables) need access to all displays, including hardware mirrors, which are not drawable.

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

