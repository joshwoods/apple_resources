

- AVFoundation
-  AVPlayerItemOutputPushDelegate 

Protocol

# AVPlayerItemOutputPushDelegate

A protocol that defines the methods to implement to respond to changes in the media data sequence.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
protocol AVPlayerItemOutputPushDelegate : NSObjectProtocol, Sendable
```

## Topics

### Flushing Sequence State

func outputSequenceWasFlushed(AVPlayerItemOutput)

Tells the delegate that the output is starting a new sequence of media data.

## Relationships

### Inherits From

- NSObjectProtocol
- Sendable

### Inherited By

- AVPlayerItemLegibleOutputPushDelegate
- AVPlayerItemMetadataOutputPushDelegate
- AVPlayerItemRenderedLegibleOutputPushDelegate

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

class AVRenderedCaptionImage

An object that provides a rendered pixel buffer and its position in pixels.

class AVPlayerItemMetadataOutput

An object that vends collections of metadata items that a player item’s tracks carry.

