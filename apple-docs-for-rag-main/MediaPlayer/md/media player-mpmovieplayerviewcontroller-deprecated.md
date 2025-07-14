

- Media Player
-  MPMoviePlayerViewController Deprecated

Class

# MPMoviePlayerViewController

A simple view controller for displaying full-screen movies.

iOS 3.2–9.0DeprecatediPadOS 3.2–9.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
@MainActor
class MPMoviePlayerViewController
```

Deprecated

Use AVPlayerViewController in AVKit.

## Overview

Important

The MPMoviePlayerViewController class is formally deprecated in iOS 9. (The MPMoviePlayerController class is also formally deprecated.) To play video content in iOS 9 and later, instead use the AVPictureInPictureController or AVPlayerViewController class from the AVKit framework, or the WKWebView class from WebKit.

Unlike using an MPMoviePlayerController object on its own to present a movie immediately, you can incorporate a movie player view controller wherever you would normally use a view controller. For example, you can present it using a tab bar or navigation bar-based interface, taking advantage of the transitions offered by those interfaces.

To present a movie player view controller modally, you typically use the presentMoviePlayerViewControllerAnimated(_:) method. This method is part of a category on the UIViewController class and is implemented by the Media Player framework. The presentMoviePlayerViewControllerAnimated(_:) method presents a movie player view controller using the standard transition animations for presenting video content. To dismiss a modally presented movie player view controller, call the dismissMoviePlayerViewControllerAnimated() method.

## Topics

### New methods

init!(contentURL: URL!)

Returns a movie player view controller initialized with the specified movie.

var moviePlayer: MPMoviePlayerController!

The movie player controller object used to present the movie.

## Relationships

### Inherits From

- UIViewController

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSExtensionRequestHandling
- NSObjectProtocol
- NSTouchBarProvider
- Sendable
- UIActivityItemsConfigurationProviding
- UIAppearanceContainer
- UIContentContainer
- UIFocusEnvironment
- UIPasteConfigurationSupporting
- UIResponderStandardEditActions
- UIStateRestoring
- UITraitChangeObservable
- UITraitEnvironment
- UIUserActivityRestoring

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

