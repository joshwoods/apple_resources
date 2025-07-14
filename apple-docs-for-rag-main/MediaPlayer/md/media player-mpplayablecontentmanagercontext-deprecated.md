

- Media Player
-  MPPlayableContentManagerContext Deprecated

Class

# MPPlayableContentManagerContext

An object representing the current state of the playable endpoint.

iOS 8.4–14.0DeprecatediPadOS 8.4–14.0DeprecatedMac Catalyst 13.1–14.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
class MPPlayableContentManagerContext
```

Deprecated

Use CarPlay framework

## Topics

### Inspecting content manager properties

var contentLimitsEnforced: Bool

A Boolean value that indicates whether the content server enforces content limits.

var endpointAvailable: Bool

Returns a Boolean that indicates whether the content server is available.

var enforcedContentItemsCount: Int

Returns the number of content items to display during content limiting.

var enforcedContentTreeDepth: Int

The maximum depth of the navigation hierarchy allowed by the content server.

var contentLimitsEnabled: Bool

A Boolean value that indicates whether the content server enables content limits.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
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

