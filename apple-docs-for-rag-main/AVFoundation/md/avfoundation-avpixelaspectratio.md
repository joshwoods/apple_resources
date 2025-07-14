

- AVFoundation
-  AVPixelAspectRatio 

Structure

# AVPixelAspectRatio

A structure that defines a pixel aspect ratio for a rendering context.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct AVPixelAspectRatio
```

## Topics

### Spacing

var horizontalSpacing: Int

The pixel aspect ratio’s horizontal spacing value.

var verticalSpacing: Int

The pixel aspect ratio’s vertical spacing value.

### Initializers

init()

Creates an empty pixel aspect ratio.

init(horizontalSpacing: Int, verticalSpacing: Int)

Creates a pixel aspect ratio with horizontal and vertical spacing values.

## Relationships

### Conforms To

- BitwiseCopyable
- Sendable

## See Also

### Getting Pixel and Edge Width Information

var edgeWidths: AVEdgeWidths

The width of the edge processing region on the left, top, right, and bottom edges, in pixels.

struct AVEdgeWidths

A structure that defines edge processing region widths.

var pixelAspectRatio: AVPixelAspectRatio

The pixel aspect ratio for rendered frames.

