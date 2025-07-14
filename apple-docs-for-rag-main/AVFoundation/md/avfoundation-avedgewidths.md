

- AVFoundation
-  AVEdgeWidths 

Structure

# AVEdgeWidths

A structure that defines edge processing region widths.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct AVEdgeWidths
```

## Topics

### Edge Widths

var left: CGFloat

The left-edge width.

var top: CGFloat

The top-edge width.

var right: CGFloat

The right-edge width.

var bottom: CGFloat

The bottom-edge width.

### Initializers

init()

Creates an empty edge widths structure.

init(left: CGFloat, top: CGFloat, right: CGFloat, bottom: CGFloat)

Creates an edge widths structure with floating-point values.

## Relationships

### Conforms To

- BitwiseCopyable
- Sendable

## See Also

### Getting Pixel and Edge Width Information

var edgeWidths: AVEdgeWidths

The width of the edge processing region on the left, top, right, and bottom edges, in pixels.

var pixelAspectRatio: AVPixelAspectRatio

The pixel aspect ratio for rendered frames.

struct AVPixelAspectRatio

A structure that defines a pixel aspect ratio for a rendering context.

