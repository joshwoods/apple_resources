

- AVFoundation
-  AVCaptionPoint 

Structure

# AVCaptionPoint

A structure that defines the origin point for a caption.

iOSiPadOSMac CatalystmacOS

``` source
struct AVCaptionPoint
```

## Topics

### Inspecting the Point

var x: AVCaptionDimension

The point’s x coordinate.

var y: AVCaptionDimension

The point’s y coordinate.

### Initializers

init()

Creates a caption dimension.

init(x: AVCaptionDimension, y: AVCaptionDimension)

Creates a caption point with x and y coordinates.

## Relationships

### Conforms To

- BitwiseCopyable
- Sendable

## See Also

### Accessing the Location

var origin: AVCaptionPoint

The region’s top-left position.

