

- Media Player
-  MPMoviePlayerController Deprecated

Class

# MPMoviePlayerController

A type of movie player that manages the playback of a movie from a file or a network stream.

iOS 3.2–9.0DeprecatediPadOS 3.2–9.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
class MPMoviePlayerController
```

Deprecated

Use AVPlayerViewController in AVKit

## Overview

Important

The MPMoviePlayerController class is formally deprecated in iOS 9. (The MPMoviePlayerViewController class is also formally deprecated.) To play video content in iOS 9 and later, instead use the AVPictureInPictureController or AVPlayerViewController class from the AVKit framework, or the WKWebView class from WebKit.

Playback occurs in a view owned by the movie player and takes place either fullscreen or inline. You can incorporate a movie player’s view into a view hierarchy owned by your app, or use an MPMoviePlayerViewController object to manage the presentation for you.

Movie players support wireless movie playback to AirPlay-enabled hardware such as Apple TV. AirPlay playback is enabled by default. To disable AirPlay in your app, set the allowsAirPlay property to false. In iOS 8.0 and later, users access AirPlay compatible hardware through the Control Panel; no AirPlay control is displayed by the movie player.

When you add a movie player’s view to your app’s view hierarchy, be sure to size the frame correctly, as shown here:

```
MPMoviePlayerController *player =
        [[MPMoviePlayerController alloc] initWithContentURL: myURL];
[player prepareToPlay];
[player.view setFrame: myView.bounds];  // player's frame must match parent's
[myView addSubview: player.view];
// ...
[player play];
```

Consider a movie player view to be an opaque structure. You can add your own custom subviews to layer content on top of the movie but you must never modify any of its existing subviews.

In addition to layering content on top of a movie, you can provide custom background content by adding subviews to the view in the backgroundView property. Custom subviews are supported in both inline and fullscreen playback modes but you must adjust the positions of your views when entering or exiting fullscreen mode. Use the MPMoviePlayerWillEnterFullscreenNotification and MPMoviePlayerWillExitFullscreenNotification notifications to detect changes to and from fullscreen mode.

This class supports programmatic control of movie playback, and user-based control via buttons supplied by the movie player. You can control most aspects of playback programmatically using the methods and properties of the MPMediaPlayback protocol, to which this class conforms. The methods and properties of that protocol let you start and stop playback, seek forward and backward through the movie’s content, and even change the playback rate. In addition, the controlStyle property of this class lets you display a set of standard system controls that allow the user to manipulate playback. You can also set the shouldAutoplay property for network-based content to start automatically.

You typically specify the movie you want to play when you create a new `MPMoviePlayerController` object. However, you can also change the currently playing movie by changing the value in the contentURL property. Changing this property lets you reuse the same movie player controller object in multiple places. For performance reasons you may want to play movies as local files. Do this by first downloading them to a local directory.

Note

Although you can create multiple `MPMoviePlayerController` objects and present their views in your interface, only one movie player at a time can play its movie.

To facilitate the creation of video bookmarks or chapter links for a long movie, the `MPMoviePlayerController` class defines methods for generating thumbnail images at specific times within a movie. You can request a single thumbnail image using the thumbnailImage(atTime:timeOption:) method or request multiple thumbnail images using the requestThumbnailImages(atTimes:timeOption:) method.

To play a network stream whose URL requires access credentials, first create an appropriate URLCredential object. Do this by calling, for example, the init(user:password:persistence:) method, as shown here:

```
NSURLCredential *credential = [[NSURLCredential alloc]
                        initWithUser: @"userName"
                            password: @"password"
                         persistence: NSURLCredentialPersistenceForSession];

self.credential = credential;
[credential release];
```

In addition, create an appropriate URLProtectionSpace object, as shown here. Make appropriate modifications for the realm you are accessing:

```
NSURLProtectionSpace *protectionSpace = [[NSURLProtectionSpace alloc]
                            initWithHost: "@streams.mydomain.com"
                                    port: 80
                                protocol: @"http"
                                   realm: @"mydomain.com"
                    authenticationMethod: NSURLAuthenticationMethodDefault];

self.protectionSpace = protectionSpace;
[protectionSpace release];
```

Add the URL credential and the protection space to the Singleton URLCredentialStorage object. Do this by calling, for example, the set(_:for:) method, as shown here:

```
[[NSURLCredentialStorage sharedCredentialStorage]
                    setDefaultCredential: credential
                      forProtectionSpace: protectionSpace];
```

With the credential and protection space information in place, you can then play the protected stream.

### Movie player notifications

A movie player generates notifications to keep your app informed about the state of movie playback. In addition to being notified when playback finishes, your app can be notified in the following situations:

- When the movie player begins playing, is paused, or begins seeking forward or backward

- When AirPlay playback starts or ends

- When the scaling mode of the movie changes

- When the movie enters or exits fullscreen mode

- When the load state for network-based movies changes

- When meta-information about the movie itself becomes available

For more information, see the Notifications section in this document.

## Topics

### Creating and initializing the object

init!(contentURL: URL!)

Returns a `MPMoviePlayerController` object initialized with the movie at the specified URL.

### Accessing movie properties

var contentURL: URL!

The URL that points to the movie file.

var movieSourceType: MPMovieSourceType

The playback type of the movie.

var movieMediaTypes: MPMovieMediaTypeMask

The types of media available in the movie.

var allowsAirPlay: Bool

Specifies whether the movie player allows AirPlay movie playback.

var isAirPlayVideoActive: Bool

Indicates whether the movie player is currently playing video via AirPlay.

var naturalSize: CGSize

The width and height of the movie frame.

var isFullscreen: Bool

A Boolean that indicates whether the movie player is in full-screen mode.

func setFullscreen(Bool, animated: Bool)

Causes the movie player to enter or exit full-screen mode.

var scalingMode: MPMovieScalingMode

The scaling mode to use when displaying the movie.

var controlStyle: MPMovieControlStyle

The style of the playback controls.

var useApplicationAudioSession: Bool

A Boolean value that indicates whether the movie player should use the app’s audio session.

### Accessing the movie duration

var duration: TimeInterval

The duration of the movie, measured in seconds.

var playableDuration: TimeInterval

The amount of currently playable content.

### Accessing the view

var view: UIView!

The view containing the movie content and controls.

var backgroundView: UIView!

A customizable view that is displayed behind the movie content.

### Controlling and monitoring playback

See also the methods of the MPMediaPlayback protocol.

var loadState: MPMovieLoadState

The network load state of the movie player.

var playbackState: MPMoviePlaybackState

The current playback state of the movie player.

var initialPlaybackTime: TimeInterval

The time, specified in seconds within the video timeline, when playback should start.

var endPlaybackTime: TimeInterval

The end time (measured in seconds) for playback of the movie.

var shouldAutoplay: Bool

A Boolean that indicates whether a movie should begin playback automatically.

var readyForDisplay: Bool

A Boolean that indicates whether the first video frame of the movie is ready to be displayed.

var repeatMode: MPMovieRepeatMode

Determines how the movie player repeats the playback of the movie.

var timedMetadata: [Any]!

Obtains the most recent time-based metadata provided by the streamed movie.

### Generating thumbnail images

func thumbnailImage(atTime: TimeInterval, timeOption: MPMovieTimeOption) -> UIImage!

Captures and returns a thumbnail image from the current movie.

func requestThumbnailImages(atTimes: [Any]!, timeOption: MPMovieTimeOption)

Captures one or more thumbnail images asynchronously from the current movie.

func cancelAllThumbnailImageRequests()

Cancels all pending asynchronous thumbnail image requests.

### Retrieving movie logs

var accessLog: MPMovieAccessLog!

A snapshot of the network playback log for the movie player if it is playing a network stream.

var errorLog: MPMovieErrorLog!

A snapshot of the playback failure error log for the movie player if it is playing a network stream.

### Constants

struct MPMovieLoadState

Constants describing the network load state of the movie player.

enum MPMovieControlStyle

Constants describing the style of the playback controls.

enum MPMovieFinishReason

Constants describing the reason that playback ended.

enum MPMoviePlaybackState

Constants describing the current playback state of the movie player.

enum MPMovieRepeatMode

Constants describing how the movie player repeats content at the end of playback.

enum MPMovieScalingMode

Constants describing how the movie content is scaled to fit the frame of its view.

enum MPMovieTimeOption

Constants describing which frame to use when generating thumbnail images.

struct MPMovieMediaTypeMask

The types of content available in the movie file.

enum MPMovieSourceType

Specifies the type of the movie file.

Thumbnail notification user info keys

The following keys may be found in the `userInfo` dictionary of a MPMoviePlayerThumbnailImageRequestDidFinishNotification notification.

Fullscreen notification keys

The following keys may be found in the `userInfo` dictionary of notifications for transitioning in or out of full-screen mode.

Playback finished notification key

The following key may be found in the userInfo dictionary of a MPMoviePlayerPlaybackDidFinishNotification notification.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- MPMediaPlayback
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

