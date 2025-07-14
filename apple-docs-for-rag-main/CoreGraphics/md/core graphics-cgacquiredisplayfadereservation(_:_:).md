

- Core Graphics
-  CGAcquireDisplayFadeReservation(\_:\_:) 

Function

# CGAcquireDisplayFadeReservation(\_:\_:)

Reserves the fade hardware for a specified time interval.

Mac Catalyst 13.1+macOS 10.2+

``` source
func CGAcquireDisplayFadeReservation(
    _ seconds: CGDisplayReservationInterval,
    _ token: UnsafeMutablePointer?
) -> CGError
```

## Parameters 

`seconds`  

The desired number of seconds to reserve the fade hardware. An application can specify any value in the interval `(0, kCGMaxDisplayReservationInterval]`.

`token`  

A pointer to storage (provided by the caller) for a fade reservation token. On return, the storage contains a new token.

## Return Value

Returns CGError.noneAvailable if another fade reservation is in effect. Otherwise, returns CGError.success.

## Discussion

Before performing a fade operation, an application must reserve the fade hardware for a specified period of time. Quartz returns a token that represents a new fade reservation. The application uses this token as an argument in subsequent calls to other display fade functions.

During the fade reservation interval, the application has exclusive rights to use the fade hardware. At the end of the interval, the token becomes invalid and the hardware automatically returns to a normal state. Typically, the application calls CGReleaseDisplayFadeReservation(_:) to release the fade reservation before it expires.

## See Also

### Functions

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

func CGDirectDisplayCopyCurrentMetalDevice(CGDirectDisplayID) -> (any MTLDevice)?

Returns the GPU device instance that’s currently driving a display.

