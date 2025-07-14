

- ScreenCaptureKit
-  SCStreamType Deprecated

Enumeration

# SCStreamType

The display type of the presented stream.

Mac Catalyst 17.0–18.0DeprecatedmacOS 14.0–15.0Deprecated

``` source
enum SCStreamType
```

Deprecated

Use SCShareableContentStyle instead

## Topics

### Client presentation

case display

The stream is currently on a complete display.

case window

The stream is currently presented as a window.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Filter properties

var contentRect: CGRect

The size and location of the content to filter, in screen points.

var pointPixelScale: Float

The scaling factor used to translate screen points into pixels.

var streamType: SCStreamType

The type of the streaming content.

Deprecated

var style: SCShareableContentStyle

The display style of the sharable content.

