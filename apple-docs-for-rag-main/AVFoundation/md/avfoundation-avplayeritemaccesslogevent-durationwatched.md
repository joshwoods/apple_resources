

- AVFoundation
- AVPlayerItemAccessLogEvent
-  durationWatched 

Instance Property

# durationWatched

The accumulated duration, in seconds, of the media played.

iOS 4.3+iPadOS 4.3+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
var durationWatched: TimeInterval { get }
```

## Discussion

The property corresponds to “c-duration-watched”.

The value of this property is negative if unknown.

This property is not compatible with key-value observing.

## See Also

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

