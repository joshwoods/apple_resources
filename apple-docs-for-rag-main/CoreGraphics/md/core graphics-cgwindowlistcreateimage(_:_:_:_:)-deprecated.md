

- Core Graphics
-  CGWindowListCreateImage(\_:\_:\_:\_:) Deprecated

Function

# CGWindowListCreateImage(\_:\_:\_:\_:)

Returns a composite image based on a dynamically generated list of windows.

``` source
func CGWindowListCreateImage(
    _ screenBounds: CGRect,
    _ listOption: CGWindowListOption,
    _ windowID: CGWindowID,
    _ imageOption: CGWindowImageOption
) -> CGImage?
```

Deprecated

Please use ScreenCaptureKit instead.

## Parameters 

`screenBounds`  

The rectangle that you want to capture. The coordinates of the rectangle must be specified in screen coordinates, where the screen origin is in the upper-left corner of the main display and y-axis values increase downward. Specify CGRectNull to indicate the minimum rectangle that encloses the specified windows. Specify CGRectInfinite to capture the entire desktop area.

`listOption`  

The options describing which windows to include in the image. Typical options let you choose all windows or windows above or below the window specified in the `windowID` parameter. For more information, see Window List Option Constants.

`windowID`  

The ID of the window to use as a reference point when determining which other windows to include in the image. For options that do not require a reference window, this parameter can be kCGNullWindowID.

`imageOption`  

The options that determine which parts of the window to capture. If you specified `CGRectNull` for the `screenBounds` parameter, these options affect the resulting bounding box used for the image. For example, if you include a window’s screen effects in the image, the bounding box may need to be slightly larger to accommodate those effects. For a list of possible options, see Window Image Types.

## Return Value

A composite image formed from the contents of the specified set of windows. If the windows are unreadable or no windows meet the specified criteria, this function returns an image that is either 0 by 0 pixels in size or is of the specified size but is filled with the transparent black color. If you call this function from outside of a GUI security session or when no window server is running, this function returns `NULL`.

## Discussion

Any windows that are onscreen but whose sharing setting is set to CGWindowSharingType.none are skipped and not included in the resulting image. If this results in no windows being available in the selected range, this function returns `NULL`.

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

