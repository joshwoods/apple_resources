

- AVFoundation
-  AVPlayerItemRenderedLegibleOutput 

Class

# AVPlayerItemRenderedLegibleOutput

A player item output that vends media with a legible characteristic as rendered pixel buffers.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+

``` source
class AVPlayerItemRenderedLegibleOutput
```

## Topics

### Creating an output

init(videoDisplay: CGSize)

Creates a rendered legible output object.

### Configuring an output

var advanceIntervalForDelegateInvocation: TimeInterval

Permits advance invocation of the associated delegate, if any.

var videoDisplaySize: CGSize

Set the video display size to use for rendering of pixel buffers.

### Setting a delegate

var delegate: (any AVPlayerItemRenderedLegibleOutputPushDelegate)?

A delegate object for this output.

func setDelegate((any AVPlayerItemRenderedLegibleOutputPushDelegate)?, queue: dispatch_queue_t?)

Sets the delegate object and the queue on which it’s invoked.

var delegateQueue: dispatch_queue_t?

The dispatch queue on which the output calls the delegate object.

protocol AVPlayerItemRenderedLegibleOutputPushDelegate

A delegate that handles the rendered pixel buffers produced by a rendered legible output object.

## Relationships

### Inherits From

- AVPlayerItemOutput

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

class AVRenderedCaptionImage

An object that provides a rendered pixel buffer and its position in pixels.

class AVPlayerItemMetadataOutput

An object that vends collections of metadata items that a player item’s tracks carry.

protocol AVPlayerItemOutputPushDelegate

A protocol that defines the methods to implement to respond to changes in the media data sequence.

