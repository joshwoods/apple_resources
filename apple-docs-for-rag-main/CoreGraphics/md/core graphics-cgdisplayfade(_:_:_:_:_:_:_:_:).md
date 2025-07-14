

- Core Graphics
-  CGDisplayFade(\_:\_:\_:\_:\_:\_:\_:\_:) 

Function

# CGDisplayFade(\_:\_:\_:\_:\_:\_:\_:\_:)

Performs a single fade operation.

Mac Catalyst 13.1+macOS 10.2+

``` source
func CGDisplayFade(
    _ token: CGDisplayFadeReservationToken,
    _ duration: CGDisplayFadeInterval,
    _ startBlend: CGDisplayBlendFraction,
    _ endBlend: CGDisplayBlendFraction,
    _ redBlend: Float,
    _ greenBlend: Float,
    _ blueBlend: Float,
    _ synchronous: boolean_t
) -> CGError
```

## Parameters 

`token`  

A reservation token for the fade hardware you acquire by calling CGAcquireDisplayFadeReservation(_:_:).

`duration`  

The desired number of seconds for the fade operation. You should use a value in the interval `[0, kCGMaxDisplayReservationInterval`\]. If the value is `0`, Quartz applies the ending blend color immediately.

`startBlend`  

An intensity value in the interval `[0, 1]` that specifies the alpha component of the desired blend color at the beginning of the fade operation. For more information, see Display Fade Blend Fractions.

`endBlend`  

An intensity value in the interval `[0, 1]` that specifies the alpha component of the desired blend color at the end of the fade operation. For more information, see Display Fade Blend Fractions.

`redBlend`  

An intensity value in the interval `[0, 1]` that specifies the red component of the desired blend color.

`greenBlend`  

An intensity value in the interval `[0, 1]` that specifies the green component of the desired blend color.

`blueBlend`  

An intensity value in the interval `[0, 1]` that specifies the blue component of the desired blend color.

`synchronous`  

Pass `true` if you want the fade operation to be synchronous; otherwise, pass `false`. If a fade operation is synchronous, the function doesn’t return until the operation is complete.

## Return Value

A result code. To interpret the result code, see CGError.

## Discussion

Over the fade operation time interval, Quartz interpolates a blending coefficient between the starting and ending values given, applying a nonlinear (sine-based) bias term. Using this coefficient, Quartz blends the video output with the specified color.

The following example shows how to perform a 2-second synchronous fade-out to black:

```
CGDisplayFade (
    myToken,
    2.0,                        // 2 seconds
    kCGDisplayBlendNormal,      // starting state
    kCGDisplayBlendSolidColor,  // ending state
    0.0, 0.0, 0.0,              // black
    true                        // wait for completion
);
```

To perform a 2-second asynchronous fade-in from black:

```
CGDisplayFade (
    myToken,
    2.0,                        // 2 seconds
    kCGDisplayBlendSolidColor,  // starting state
    kCGDisplayBlendNormal,      // ending state
    0.0, 0.0, 0.0,              // black
    false                       // don't wait for completion
);
```

If you specify an asynchronous fade operation, it’s safe to call CGReleaseDisplayFadeReservation(_:) immediately after this function returns.

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

