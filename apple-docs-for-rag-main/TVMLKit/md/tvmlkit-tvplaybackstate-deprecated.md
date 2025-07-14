

- TVMLKit
-  TVPlaybackState Deprecated

Enumeration

# TVPlaybackState

The possible states of a player.

tvOS 12.0–18.0Deprecated

``` source
enum TVPlaybackState
```

Deprecated

Please use SwiftUI or UIKit

## Topics

### Playback States

case undefined

The playback state of the player is undefined.

case begin

The player is beginning playback.

case loading

The player is loading a media item.

case playing

The player is currently playing.

case paused

The player paused playback.

case scanning

The player is quickly scanning forwards or backwards.

case fastForwarding

The player is fast-forwarding.

case rewinding

The player is rewinding.

case end

The player ended playback.

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

### Controlling Playback

func next()

Plays the next media item in the playlist.

Deprecated

func pause()

Pauses the currently playing item.

Deprecated

func previous()

Plays the previous media item in the playlist.

Deprecated

var state: TVPlaybackState

The current state of the player.

Deprecated

func dispatch(event: TVPlaybackEvent, userInfo: (any TVPlaybackEventMarshaling)?, completion: ((Bool) -> Void)?)

Dispatches custom playback events to the JavaScript environment.

Deprecated

struct TVPlaybackEvent

Extend this structure to send your custom playback events to the JavaScript environment.

Deprecated

protocol TVPlaybackEventMarshaling

A protocol used for sending and receiving information across the JavaScript bridge.

Deprecated

class TVPlaybackCustomEventUserInfo

The user information used in a custom playback event.

Deprecated

