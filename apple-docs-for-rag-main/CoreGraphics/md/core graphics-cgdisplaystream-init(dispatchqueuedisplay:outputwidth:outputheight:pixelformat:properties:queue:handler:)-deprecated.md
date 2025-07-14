

- Core Graphics
- CGDisplayStream
-  init(dispatchQueueDisplay:outputWidth:outputHeight:pixelFormat:properties:queue:handler:) Deprecated

Initializer

# init(dispatchQueueDisplay:outputWidth:outputHeight:pixelFormat:properties:queue:handler:)

Creates a new display stream whose updates are delivered to a dispatch queue.

``` source
init?(
    dispatchQueueDisplay display: CGDirectDisplayID,
    outputWidth: Int,
    outputHeight: Int,
    pixelFormat: Int32,
    properties: CFDictionary?,
    queue: dispatch_queue_t,
    handler: CGDisplayStreamFrameAvailableHandler?
)
```

Deprecated

Please use ScreenCaptureKit instead.

## Parameters 

`display`  

The identifier of the display to be streamed.

`outputWidth`  

The width of the output frames in pixels. The width must not be zero.

`outputHeight`  

The height of the output frames in pixels. The height must not be zero.

`pixelFormat`  

The desired Core Media pixel format of the output frame data. The value must be one of the following:

- `'BGRA'`: Packed Little Endian ARGB8888

- `'l10r'`: Packed Little Endian ARGB2101010

- `'420v'`: 2-plane “video” range YCbCr 4:2:0

- `'420f'`: 2-plane “full” range YCbCr 4:2:0

`properties`  

A dictionary of optional properties for the display stream. See Display Stream Optional Property Keys for the possible keys and values that can be provided in the options dictionary.

`queue`  

The GCD dispatch queue used when calling the update handler.

`handler`  

A block to be called when new frames are ready.

## Return Value

A new `CGDisplayStream` object.

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

