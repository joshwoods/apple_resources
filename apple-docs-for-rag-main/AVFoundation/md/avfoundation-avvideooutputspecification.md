

- AVFoundation
-  AVVideoOutputSpecification 

Class

# AVVideoOutputSpecification

An object that specifies the pixel buffer attributes and tag collections handled by a player video output.

iOS 17.2+iPadOS 17.2+Mac Catalyst 17.2+macOS 14.2+tvOS 17.2+visionOS 1.1+watchOS 10.2+

``` source
class AVVideoOutputSpecification
```

## Topics

### Creating a specification

convenience init(tagCollections: [[CMTag]])

### Configuring the specification

var defaultOutputSettings: [String : any Sendable]?

func setOutputSettings([String : any Sendable]?, for: [CMTag])

var defaultPixelBufferAttributes: [String : Any]?

func setOutputPixelBufferAttributes([String : Any]?, for: [CMTag])

var preferredTagCollections: [[CMTag]]

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

## See Also

### Media output

class AVPlayerVideoOutput

An object that receives video data from a player object.

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

protocol AVPlayerItemOutputPushDelegate

A protocol that defines the methods to implement to respond to changes in the media data sequence.

