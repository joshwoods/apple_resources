

- Media Player
-  MPMoviePlaybackState Deprecated

Enumeration

# MPMoviePlaybackState

Constants describing the current playback state of the movie player.

iOS 3.2–9.0DeprecatediPadOS 3.2–9.0DeprecatedMac Catalyst 13.1–13.1DeprecatedtvOSDeprecatedvisionOS 1.0–1.0Deprecated

``` source
enum MPMoviePlaybackState
```

Deprecated

Use AVPlayerViewController in AVKit

## Topics

### Constants

case stopped

case playing

case paused

case interrupted

case seekingForward

case seekingBackward

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Constants

struct MPMovieLoadState

Constants describing the network load state of the movie player.

Deprecated

enum MPMovieControlStyle

Constants describing the style of the playback controls.

Deprecated

enum MPMovieFinishReason

Constants describing the reason that playback ended.

Deprecated

enum MPMovieRepeatMode

Constants describing how the movie player repeats content at the end of playback.

Deprecated

enum MPMovieScalingMode

Constants describing how the movie content is scaled to fit the frame of its view.

Deprecated

enum MPMovieTimeOption

Constants describing which frame to use when generating thumbnail images.

Deprecated

struct MPMovieMediaTypeMask

The types of content available in the movie file.

Deprecated

enum MPMovieSourceType

Specifies the type of the movie file.

Deprecated

Thumbnail notification user info keys

The following keys may be found in the `userInfo` dictionary of a MPMoviePlayerThumbnailImageRequestDidFinishNotification notification.

Fullscreen notification keys

The following keys may be found in the `userInfo` dictionary of notifications for transitioning in or out of full-screen mode.

Playback finished notification key

The following key may be found in the userInfo dictionary of a MPMoviePlayerPlaybackDidFinishNotification notification.

