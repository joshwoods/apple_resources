

- Media Player
-  MPMovieAccessLog Deprecated

Class

# MPMovieAccessLog

Key metrics about network playback for an associated movie player that’s playing streamed content.

iOS 4.3–9.0DeprecatediPadOS 4.3–9.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
class MPMovieAccessLog
```

Deprecated

Use AVFoundation.

## Overview

The log presents these metrics as a collection of MPMovieAccessLogEvent instances and also makes it available in a textual format. A movie access log describes one uninterrupted period of playback. A movie player (an instance of the MPMoviePlayerController class) can access this log from its accessLog property. All movie access log properties are read-only.

## Topics

### Movie access log properties

var extendedLogData: Data!

A textual version of the web server access log for the associated movie player.

var extendedLogDataStringEncoding: UInt

The string encoding for the extendedLogData property.

var events: [Any]!

The events in the movie access log.

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

class MPMovieAccessLogEvent

A single piece of information for a movie access log.

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

