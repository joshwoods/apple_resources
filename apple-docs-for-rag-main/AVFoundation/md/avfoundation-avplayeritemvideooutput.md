

- AVFoundation
-  AVPlayerItemVideoOutput 

Class

# AVPlayerItemVideoOutput

An object that outputs video frames from a player item.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+

``` source
class AVPlayerItemVideoOutput
```

## Topics

### Creating a Video Output

init(pixelBufferAttributes: [String : Any]?)

Creates a video output object using the specified pixel buffer attributes.

init(outputSettings: [String : Any]?)

Creates a video output object initialized with the specified output settings.

### Configuring the Delegate

func setDelegate((any AVPlayerItemOutputPullDelegate)?, queue: dispatch_queue_t?)

Sets the delegate and dispatch queue for the receiver.

var delegate: (any AVPlayerItemOutputPullDelegate)?

The delegate for the video output object.

protocol AVPlayerItemOutputPullDelegate

Methods you can implement to respond to pixel buffer changes.

var delegateQueue: dispatch_queue_t?

The dispatch queue on which to call delegate methods.

### Notifying the Delegate of Changes

func requestNotificationOfMediaDataChange(withAdvanceInterval: TimeInterval)

Tells the receiver that the video out put client is entering a quiescent state.

### Getting Pixel Buffer Data

func hasNewPixelBuffer(forItemTime: CMTime) -> Bool

Returns a Boolean value that indicates whether video output is available for the specified item time.

func copyPixelBuffer(forItemTime: CMTime, itemTimeForDisplay: UnsafeMutablePointer&lt;CMTime>?) -> CVPixelBuffer?

Retrieves an image that is appropriate for display at the specified item time, and marks the image as acquired.

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

class AVPlayerItemLegibleOutput

An object that vends attributed strings for media with a legible characteristic.

class AVPlayerItemRenderedLegibleOutput

A player item output that vends media with a legible characteristic as rendered pixel buffers.

class AVRenderedCaptionImage

An object that provides a rendered pixel buffer and its position in pixels.

class AVPlayerItemMetadataOutput

An object that vends collections of metadata items that a player item’s tracks carry.

protocol AVPlayerItemOutputPushDelegate

A protocol that defines the methods to implement to respond to changes in the media data sequence.

