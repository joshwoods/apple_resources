

- Media Player
-  MPMovieErrorLogEvent Deprecated

Class

# MPMovieErrorLogEvent

A single piece of information for a movie error log.

iOS 4.3–9.0DeprecatediPadOS 4.3–9.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
class MPMovieErrorLogEvent
```

Deprecated

Use AVFoundation.

## Overview

All movie error log event properties are read-only. For a description of movie error logs, see MPMovieErrorLog.

## Topics

### Movie error log event properties

var date: Date!

The date and time when the error occurred.

var uri: String!

The URI of the item playing when the error occurred.

var serverAddress: String!

The IP address of the web server that was the source of the error.

var playbackSessionID: String!

A globally unique identifier (GUID) for the playback session.

var errorStatusCode: Int

A unique error code identifier.

var errorDomain: String!

The network domain of the error.

var errorComment: String!

A description of the error.

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

class MPMovieAccessLogEvent

A single piece of information for a movie access log.

Deprecated

class MPMovieErrorLog

Data describing network resource playback failures for the associated movie player, including timestamps indicating when each failure occurred.

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

