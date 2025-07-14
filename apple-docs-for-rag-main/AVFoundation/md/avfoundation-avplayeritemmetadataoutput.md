

- AVFoundation
-  AVPlayerItemMetadataOutput 

Class

# AVPlayerItemMetadataOutput

An object that vends collections of metadata items that a player item’s tracks carry.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
class AVPlayerItemMetadataOutput
```

## Overview

Note

Setting the value of suppressesPlayerRendering on an instance of `AVPlayerItemMetadataOutput` has no effect.

## Topics

### Creating a Metadata Output

init(identifiers: [String]?)

Creates an instance of AVPlayerItemMetadataOutput.

### Configuring the Delegate

var advanceIntervalForDelegateInvocation: TimeInterval

The time interval, in seconds, the player item metadata output object messages its delegate earlier than normal.

var delegate: (any AVPlayerItemMetadataOutputPushDelegate)?

The delegate object.

protocol AVPlayerItemMetadataOutputPushDelegate

Methods you can implement to provide additional metadata.

var delegateQueue: dispatch_queue_t?

The dispatch queue on which messages are sent to the delegate.

func setDelegate((any AVPlayerItemMetadataOutputPushDelegate)?, queue: dispatch_queue_t?)

Sets the delegate and a dispatch queue on which the delegate is called.

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

class AVPlayerItemRenderedLegibleOutput

A player item output that vends media with a legible characteristic as rendered pixel buffers.

class AVRenderedCaptionImage

An object that provides a rendered pixel buffer and its position in pixels.

protocol AVPlayerItemOutputPushDelegate

A protocol that defines the methods to implement to respond to changes in the media data sequence.

