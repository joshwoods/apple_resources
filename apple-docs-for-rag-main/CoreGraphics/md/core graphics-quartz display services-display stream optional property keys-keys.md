

- Core Graphics
- Quartz Display Services
-  Display Stream Optional Property Keys 

API Collection

# Display Stream Optional Property Keys

These keys are used to populate the `properties` dictionary used when creating a new display stream.

## Topics

### Constants

class let sourceRect: CFString

This key specifies that the display stream only samples a subset of the display’s framebuffer.

Deprecated

class let destinationRect: CFString

This key specifies that the display stream outputs the frame data into a subset of the output `IOSurface` object.

Deprecated

class let preserveAspectRatio: CFString

This key specifies whether the display stream preserves the aspect ratio of the source pixel data. If this key is not included in the dictionary, then the aspect ratio is preserved. If the aspect ratio is preserved, then the display stream adds black bars to the output data. If the aspect ratio is not preserved, then the pixel data is stretched to fit the output buffer’s dimensions. The value associated with the key must be a `CFBoolean`.

Deprecated

class let colorSpace: CFString

This key specifies the color space of the output buffer. If this key is not included in the dictionary, the output buffer uses the same color space as the display. The value associated with this key must be a CGColorSpace for the desired color space.

Deprecated

class let minimumFrameTime: CFString

This key specifies the desired minimum time between frame updates, allowing you to throttle the rate at which updates are received. If this key is not included in the dictionary, the default value is `0`, meaning that updates are not throttled. The value must be specified as a `CFNumber`.

Deprecated

class let showCursor: CFString

This key specifies whether the cursor should appear in the stream. If this key is not included in the dictionary, the cursor is visible. The value must be specified as a `CFBoolean`.

Deprecated

class let queueDepth: CFString

This key specifies the number of frames to keep in the queue. If this key is not included in the dictionary, the default value is `3` frames. Specifying more frames uses more memory, but may allow you to process frame data without stalling the display stream. The value associated with this key should be specified as a `CFNumber`, and should not exceed `8` frames.

Deprecated

class let yCbCrMatrix: CFString

This key should only be included if you the display stream is creating output frames in either the 420v or 420f formats. It is used to specify the YCbCr matrix applied to the output surface.

Deprecated

## See Also

### Constants

struct CGCaptureOptions

Configuration parameters that are used when capturing displays.

struct CGDisplayChangeSummaryFlags

The configuration parameters that are passed to a display reconfiguration callback function.

struct CGConfigureOption

The scope of the changes in a display configuration transaction.

Display Fade Blend Fractions

The lower and upper bounds for blend color fractions during a display fade operation.

Display Fade Constants

Values relating to fade operations.

Display ID Defaults

Default values for a display ID.

Display Mode Standard Properties

Keys for the standard properties in a display mode dictionary.

Display Mode Optional Properties

Keys for optional properties in a display mode dictionary.

Reserved Window Levels

Window level constants.

struct CGScreenUpdateOperation

Types of screen-update operations.

enum CGWindowLevelKey

Keys that represent the standard window levels in macOS. Quartz includes these keys to support application frameworks like Cocoa. Applications do not need to use them directly.

Window Server Session Properties

The keys for the standard properties in a window server session dictionary.

enum CGDisplayStreamUpdateRectType

Use these constants to determine which rectangles your app is interested in.

enum CGDisplayStreamFrameStatus

Describes a frame update event.

Display Stream YCbCr to RGB conversion Matrix Options

These strings are used to specify a matrix for the yCbCrMatrix option.

