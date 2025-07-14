

- Media Player
-  MPMovieAccessLogEvent Deprecated

Class

# MPMovieAccessLogEvent

A single piece of information for a movie access log.

iOS 4.3–9.0DeprecatediPadOS 4.3–9.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
class MPMovieAccessLogEvent
```

Deprecated

Use AVFoundation.

## Overview

For a description of movie access logs, see MPMovieAccessLog.

## Topics

### Movie access log event properties

var numberOfSegmentsDownloaded: Int

A count of media segments downloaded from the web server to your app.

var playbackStartDate: Date!

The timestamp for when playback began for the movie log access event.

var uri: String!

The URI of the playback item.

var serverAddress: String!

The IPv4 or IPv6 address of the web server that was the source of the last delivered media segment.

var numberOfServerAddressChanges: Int

A count of changes to the serverAddress property over the last uninterrupted period of playback.

var playbackSessionID: String!

A GUID that identifies the playback session to use in HTTP requests.

var playbackStartOffset: TimeInterval

An offset into the playlist where the last uninterrupted period of playback began, in seconds.

var segmentsDownloadedDuration: TimeInterval

The accumulated duration of the media downloaded, in seconds.

var durationWatched: TimeInterval

The accumulated duration of the media played, in seconds.

var numberOfStalls: Int

The total number of playback stalls encountered.

var numberOfBytesTransferred: Int64

The accumulated number of bytes transferred.

var observedBitrate: Double

The empirical throughput across all media downloaded for the movie player, in bits per second.

var indicatedBitrate: Double

The throughput required to play the stream, as advertised by the web server, in bits per second.

var numberOfDroppedVideoFrames: Int

The total number of dropped video frames.

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

### Deprecated symbols

class MPMovieAccessLog

Key metrics about network playback for an associated movie player that’s playing streamed content.

Deprecated

class MPMovieErrorLog

Data describing network resource playback failures for the associated movie player, including timestamps indicating when each failure occurred.

Deprecated

class MPMovieErrorLogEvent

A single piece of information for a movie error log.

Deprecated

struct MPMovieLoadState

Constants describing the network load state of the movie player.

Deprecated

struct MPMovieMediaTypeMask

The types of content available in the movie file.

Deprecated

class MPMoviePlayerController

A type of movie player that manages the playback of a movie from a file or a network stream.

Deprecated

class MPMoviePlayerViewController

A simple view controller for displaying full-screen movies.

Deprecated

class MPTimedMetadata

A *timed metadata object that* carries time-based information within HTTP streamed media.

Deprecated

class MPPlayableContentManager

A shared content manager for controlling interactions between your media app and system-provided or external media player interfaces.

Deprecated

class MPPlayableContentManagerContext

An object representing the current state of the playable endpoint.

Deprecated

class var iPodMusicPlayer: MPMusicPlayerController

Returns the iPod music player, which controls the iPod app’s state.

Deprecated

convenience init(image: UIImage)

Initializes a media item artwork instance with a full-size image.

Deprecated

var imageCropRect: CGRect

The bounds, in points, of the content area for the full size image associated with the media item artwork.

Deprecated

var showsRouteButton: Bool

A Boolean value that indicates whether the route button is visible in the volume view.

Deprecated

func routeButtonImage(for: UIControl.State) -> UIImage?

Returns the button image associated with the specified control state.

Deprecated

