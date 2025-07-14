

- Media Player
-  MPPlayableContentManager Deprecated

Class

# MPPlayableContentManager

A shared content manager for controlling interactions between your media app and system-provided or external media player interfaces.

iOS 7.1–14.0DeprecatediPadOS 7.1–14.0DeprecatedMac Catalyst 13.1–14.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
class MPPlayableContentManager
```

Deprecated

Use CarPlay framework

## Overview

Important

Some features of this class are specific to CarPlay, which requires a special entitlement issued by Apple. Apps without the correct entitlement won’t appear on the CarPlay home screen. See http://www.apple.com/ios/carplay/ for more information.

The app provides data to the content manager so that the media player can browse the content provided. A delegate provides the media player the ability to perform actions that manage the app’s playback queue.

You don’t create a new content manager directly, instead you grab the shared content manager using the shared() method. After getting the shared content manager, your next step depends on the features your app supports:

- To provide content navigation and suggested content for CarPlay, immediately set both the dataSource and delegate properties. After setting these properties, use the beginUpdates() and endUpdates() methods to load the information from the data source.

- To provide suggested content when the user connects headphones, a Bluetooth stereo, or another output device, set only the delegate property. After you set a delegate, iOS automatically calls methods in the MPPlayableContentDelegate protocol allowing you to suggest appropriate content.

## Topics

### Providing playable content

var dataSource: (any MPPlayableContentDataSource)?

The data source provided by the app.

protocol MPPlayableContentDataSource

The data source providing media metadata to external media players so they can build user interfaces displaying your app’s content.

### Responding to playback events

var delegate: (any MPPlayableContentDelegate)?

A delegate that lets the media player manage the app’s playback queue.

protocol MPPlayableContentDelegate

The protocol used to let external media players send playback commands to an app.

### Setting the content manager

class func shared() -> Self

Returns the current content manager instance.

### Updating data

func beginUpdates()

Updates several Media Player content items at once.

func endUpdates()

Ends a synchronized update.

func reloadData()

Reloads the data from the data source.

### Retrieving information on currently playing items

var context: MPPlayableContentManagerContext

The current state of the playable content endpoint.

var nowPlayingIdentifiers: [String]

The content items currently playing based on their identifiers.

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

