

- Core Graphics
-  CGWindowListCopyWindowInfo(\_:\_:) 

Function

# CGWindowListCopyWindowInfo(\_:\_:)

Generates and returns information about the selected windows in the current user session.

Mac Catalyst 13.1+macOS 10.5+

``` source
func CGWindowListCopyWindowInfo(
    _ option: CGWindowListOption,
    _ relativeToWindow: CGWindowID
) -> CFArray?
```

## Parameters 

`option`  

The options describing which window dictionaries to return. Typical options let you return dictionaries for all windows or for windows above or below the window specified in the `relativeToWindow` parameter. For more information, see Window List Option Constants.

`relativeToWindow`  

The ID of the window to use as a reference point when determining which other window dictionaries to return. For options that do not require a reference window, this parameter can be kCGNullWindowID.

## Return Value

An array of CFDictionary types, each of which contains information about one of the windows in the current user session. If there are no windows matching the desired criteria, the function returns an empty array. If you call this function from outside of a GUI security session or when no window server is running, this function returns `NULL`.

## Discussion

You can use this function to get detailed information about the configuration of one or more windows in the current user session. For example, you can use this function to get the bounds of the window, its window ID, and information about how it is managed by the window server. For the list of keys and values that may be present in the dictionary, see Required Window List Keys and Optional Window List Keys.

Generating the dictionaries for system windows is a relatively expensive operation. As always, you should profile your code and adjust your usage of this function appropriately for your needs.

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

