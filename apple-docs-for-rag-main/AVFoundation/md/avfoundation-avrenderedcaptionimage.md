

- AVFoundation
-  AVRenderedCaptionImage 

Class

# AVRenderedCaptionImage

An object that provides a rendered pixel buffer and its position in pixels.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+

``` source
class AVRenderedCaptionImage
```

## Topics

### Inspecting the image

var pixelBuffer: CVPixelBuffer

An object that contains pixel data for the rendered caption.

var position: CGPoint

A point that defines the position, in pixels, of the rendered caption image relative to the video frame.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Media output

class AVPlayerVideoOutput

An object that receives video data from a player object.

class AVVideoOutputSpecification

An object that specifies the pixel buffer attributes and tag collections handled by a player video output.

class AVPlayerItemOutput

An abstract class that defines the common interface to output media data from a player item.

class AVPlayerItemVideoOutput

An object that outputs video frames from a player item.

class AVPlayerItemLegibleOutput

An object that vends attributed strings for media with a legible characteristic.

class AVPlayerItemRenderedLegibleOutput

A player item output that vends media with a legible characteristic as rendered pixel buffers.

class AVPlayerItemMetadataOutput

An object that vends collections of metadata items that a player item’s tracks carry.

protocol AVPlayerItemOutputPushDelegate

A protocol that defines the methods to implement to respond to changes in the media data sequence.

