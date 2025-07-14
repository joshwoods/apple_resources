

- AVFoundation
- AVPlayerItemAccessLogEvent
-  numberOfSegmentsDownloaded Deprecated

Instance Property

# numberOfSegmentsDownloaded

A count of the media segments downloaded from the server to this client.

tvOS 9.0–9.0Deprecated

``` source
var numberOfSegmentsDownloaded: Int { get }
```

## Discussion

The property corresponds to “sc-count”.

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

var durationWatched: TimeInterval

The accumulated duration, in seconds, of the media played.

var numberOfDroppedVideoFrames: Int

The total number of dropped video frames

var numberOfStalls: Int

The total number of playback stalls encountered.

var segmentsDownloadedDuration: TimeInterval

The accumulated duration, in seconds, of the media segments downloaded.

var downloadOverdue: Int

The total number of times that downloading the segments took too long.

