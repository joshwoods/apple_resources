

- Media Player
- MPMovieAccessLogEvent
-  durationWatched Deprecated

Instance Property

# durationWatched

The accumulated duration of the media played, in seconds.

iOS 3.2–9.0DeprecatediPadOS 3.2–9.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
var durationWatched: TimeInterval { get }
```

Deprecated

Use AVPlayerViewController in AVKit

## See Also

### Movie access log event properties

var numberOfSegmentsDownloaded: Int

A count of media segments downloaded from the web server to your app.

Deprecated

var playbackStartDate: Date!

The timestamp for when playback began for the movie log access event.

Deprecated

var uri: String!

The URI of the playback item.

Deprecated

var serverAddress: String!

The IPv4 or IPv6 address of the web server that was the source of the last delivered media segment.

Deprecated

var numberOfServerAddressChanges: Int

A count of changes to the serverAddress property over the last uninterrupted period of playback.

Deprecated

var playbackSessionID: String!

A GUID that identifies the playback session to use in HTTP requests.

Deprecated

var playbackStartOffset: TimeInterval

An offset into the playlist where the last uninterrupted period of playback began, in seconds.

Deprecated

var segmentsDownloadedDuration: TimeInterval

The accumulated duration of the media downloaded, in seconds.

Deprecated

var numberOfStalls: Int

The total number of playback stalls encountered.

Deprecated

var numberOfBytesTransferred: Int64

The accumulated number of bytes transferred.

Deprecated

var observedBitrate: Double

The empirical throughput across all media downloaded for the movie player, in bits per second.

Deprecated

var indicatedBitrate: Double

The throughput required to play the stream, as advertised by the web server, in bits per second.

Deprecated

var numberOfDroppedVideoFrames: Int

The total number of dropped video frames.

Deprecated

