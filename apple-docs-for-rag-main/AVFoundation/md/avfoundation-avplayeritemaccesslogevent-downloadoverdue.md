

- AVFoundation
- AVPlayerItemAccessLogEvent
-  downloadOverdue 

Instance Property

# downloadOverdue

The total number of times that downloading the segments took too long.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
var downloadOverdue: Int { get }
```

## Discussion

The value of the property is negative if unknown.

This property corresponds to “c-overdue”.

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

