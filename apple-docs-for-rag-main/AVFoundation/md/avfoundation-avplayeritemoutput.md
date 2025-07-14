

- AVFoundation
-  AVPlayerItemOutput 

Class

# AVPlayerItemOutput

An abstract class that defines the common interface to output media data from a player item.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
class AVPlayerItemOutput
```

## Overview

This class provides basic methods for converting time values to the timebase of the item. It also provides an option to suppress rendering of the output associated with the specific instance of this class.

Important

Don’t create instances of this class directly but instead use one of the concrete subclasses that manage specific types of assets.

## Topics

### Time Conversion

func itemTime(forHostTime: CFTimeInterval) -> CMTime

Converts a host time, specified in seconds, to the item’s timebase.

func itemTime(forMachAbsoluteTime: Int64) -> CMTime

Converts a Mach host time to the item’s timebase.

func itemTime(for: CVTimeStamp) -> CMTime

Converts a Core Video timestamp to the item’s timebase.

### Configuring the Playback Options

var suppressesPlayerRendering: Bool

A Boolean value that indicates whether the player object renders the receiver’s output.

## Relationships

### Inherits From

- NSObject

### Inherited By

- AVPlayerItemLegibleOutput
- AVPlayerItemMetadataOutput
- AVPlayerItemRenderedLegibleOutput
- AVPlayerItemVideoOutput

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

