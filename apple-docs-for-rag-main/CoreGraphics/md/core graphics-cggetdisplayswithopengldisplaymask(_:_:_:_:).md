

- Core Graphics
-  CGGetDisplaysWithOpenGLDisplayMask(\_:\_:\_:\_:) 

Function

# CGGetDisplaysWithOpenGLDisplayMask(\_:\_:\_:\_:)

Provides a list of displays that corresponds to the bits set in an OpenGL display mask.

Mac Catalyst 13.1+macOS 10.0+

``` source
func CGGetDisplaysWithOpenGLDisplayMask(
    _ mask: CGOpenGLDisplayMask,
    _ maxDisplays: UInt32,
    _ displays: UnsafeMutablePointer?,
    _ matchingDisplayCount: UnsafeMutablePointer?
) -> CGError
```

## Parameters 

`mask`  

An OpenGL display mask that identifies one or more displays.

`maxDisplays`  

The size of the `displays` array. This value determines the maximum number of displays the list includes.

`displays`  

A pointer to storage you provide for an array of display IDs. On return, the array contains a list of displays that corresponds to the bits set in the mask. If you pass `NULL`, on return the display count contains the total number of displays specified in the mask.

`matchingDisplayCount`  

A pointer to a display count variable you provide. On return, the display count contains the actual number of displays the function added to the `displays` array. This value is at most `maxDisplays`.

## Return Value

A result code. To interpret the result code, see CGError.

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

