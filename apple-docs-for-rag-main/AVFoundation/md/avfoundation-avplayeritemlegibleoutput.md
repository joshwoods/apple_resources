

- AVFoundation
-  AVPlayerItemLegibleOutput 

Class

# AVPlayerItemLegibleOutput

An object that vends attributed strings for media with a legible characteristic.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
class AVPlayerItemLegibleOutput
```

## Topics

### Creating a Legible Output

init(mediaSubtypesForNativeRepresentation: [NSNumber])

Creates an initialized legible-output object.

### Configuring Text Styling

var textStylingResolution: AVPlayerItemLegibleOutput.TextStylingResolution

A string identifier indicating the degree of text styling to be applied to attributed strings vended by the object.

struct TextStylingResolution

A text styling resolution.

### Configuring the Delegate

var delegate: (any AVPlayerItemLegibleOutputPushDelegate)?

The delegate of the output class.

func setDelegate((any AVPlayerItemLegibleOutputPushDelegate)?, queue: dispatch_queue_t?)

Sets the receiver’s delegate and a dispatch queue on which the delegate is called.

protocol AVPlayerItemLegibleOutputPushDelegate

Methods you can implement to provide alternative attributed-string output.

var advanceIntervalForDelegateInvocation: TimeInterval

The time interval, in seconds, that a player item legible output object messages its delegate earlier than normal.

var delegateQueue: dispatch_queue_t?

The dispatch queue on which the delegate is called.

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

class AVPlayerItemRenderedLegibleOutput

A player item output that vends media with a legible characteristic as rendered pixel buffers.

class AVRenderedCaptionImage

An object that provides a rendered pixel buffer and its position in pixels.

class AVPlayerItemMetadataOutput

An object that vends collections of metadata items that a player item’s tracks carry.

protocol AVPlayerItemOutputPushDelegate

A protocol that defines the methods to implement to respond to changes in the media data sequence.

