

- Media Player
-  MPTimedMetadata Deprecated

Class

# MPTimedMetadata

A *timed metadata object that* carries time-based information within HTTP streamed media.

iOS 4.0–9.0DeprecatediPadOS 4.0–9.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
class MPTimedMetadata
```

Deprecated

Use AVFoundation.

## Overview

Content providers can embed these objects when creating a stream. The properties and constants in this class let you extract the metadata as you play the stream using an MPMoviePlayerController object. For example, the provider of a live sports video stream could use `MPTimedMetadata` instances to embed game scores, with timestamps, in the stream. On the client side—that is, on the user’s device—their application could employ the properties of this class to update their app’s user interface in real time during the game.

A Javascript implementation of this class is also available for use by web-based applications.

## Topics

### Extracting timed metadata from a stream

var allMetadata: [AnyHashable : Any]!

A dictionary containing all the metadata in the object.

var key: String!

A key that identifies a piece of timed metadata.

var keyspace: String!

The namespace of the identifying key.

var timestamp: TimeInterval

The timestamp of the metadata, in the timebase of the media stream.

var value: Any!

The timed metadata.

### Constants

Timed metadata dictionary keys

Dictionary keys for use with the allMetadata property. All keys are optional.

### Notifications

let MPMoviePlayerTimedMetadataUserInfoKey: String

An NSDictionary object containing the most recent `MPTimedMetadata` objects.

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

