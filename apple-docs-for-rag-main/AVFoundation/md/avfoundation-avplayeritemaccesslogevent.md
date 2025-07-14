

- AVFoundation
-  AVPlayerItemAccessLogEvent 

Class

# AVPlayerItemAccessLogEvent

A single entry in a player item’s access log.

iOS 4.3+iPadOS 4.3+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
class AVPlayerItemAccessLogEvent
```

## Overview

This object provides named properties for accessing the data fields of each log event. Each event is a single entry in an AVPlayerItem object’s access log.

These properties aren’t observable. For more information about key-value observing, see Using Key-Value Observing in Swift.

## Topics

### Getting Server-Related Log Events

var uri: String?

The URI of the playback item.

var serverAddress: String?

The IP address of the server that was the source of the last delivered media segment.

var numberOfServerAddressChanges: Int

A count of changes to the server address over the last uninterrupted period of playback.

var mediaRequestsWWAN: Int

The number of network read requests over a WWAN.

var transferDuration: TimeInterval

The accumulated duration, in seconds, of active network transfer of bytes.

var numberOfBytesTransferred: Int64

The accumulated number of bytes transferred by the item.

var numberOfMediaRequests: Int

The number of media read requests from the server to this client.

### Getting Playback-Related Log Events

var playbackStartDate: Date?

The date and time at which playback began for this event.

var playbackSessionID: String?

A GUID that identifies the playback session.

var playbackStartOffset: TimeInterval

The offset, in seconds, in the playlist where the last uninterrupted period of playback began.

var playbackType: String?

The playback type.

var startupTime: TimeInterval

The accumulated duration, in seconds, until the player item is ready to play.

var durationWatched: TimeInterval

The accumulated duration, in seconds, of the media played.

var numberOfDroppedVideoFrames: Int

The total number of dropped video frames

var numberOfStalls: Int

The total number of playback stalls encountered.

var numberOfSegmentsDownloaded: Int

A count of the media segments downloaded from the server to this client.

Deprecated

var segmentsDownloadedDuration: TimeInterval

The accumulated duration, in seconds, of the media segments downloaded.

var downloadOverdue: Int

The total number of times that downloading the segments took too long.

### Getting Bit Rate Log Events

The observed properties measure actual network download performance and indicated properties measure the bit rate of the media.

var observedBitrateStandardDeviation: Double

The standard deviation of the observed segment download bit rates.

var observedMaxBitrate: Double

The maximum observed segment download bit rate.

Deprecated

var observedMinBitrate: Double

The minimum observed segment download bit rate.

Deprecated

var switchBitrate: Double

The bandwidth value that causes a switch, up or down, in the item’s quality being played.

var indicatedBitrate: Double

The throughput, in bits per second, required to play the stream, as advertised by the server.

var observedBitrate: Double

The empirical throughput, in bits per second, across all media downloaded.

var averageAudioBitrate: Double

The audio track’s average bit rate, in bits per second.

var averageVideoBitrate: Double

The video track’s average bit rate, in bits per second.

var indicatedAverageBitrate: Double

The average throughput, in bits per second, required to play the stream, as advertised by the server.

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
- Sendable

## See Also

### Accessing Logging Information

func accessLog() -> AVPlayerItemAccessLog?

Returns an object that represents a snapshot of the network access log.

class AVPlayerItemAccessLog

An object used to retrieve the access log associated with a player item.

func errorLog() -> AVPlayerItemErrorLog?

Returns an object that represents a snapshot of the error log.

class AVPlayerItemErrorLog

The error log associated with a player item.

class AVPlayerItemErrorLogEvent

A single item in a player item’s error log.

