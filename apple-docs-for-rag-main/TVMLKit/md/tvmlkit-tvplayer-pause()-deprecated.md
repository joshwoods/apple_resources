

- TVMLKit
- TVPlayer
-  pause() Deprecated

Instance Method

# pause()

Pauses the currently playing item.

tvOS 12.0–18.0Deprecated

``` source
func pause()
```

Deprecated

Please use SwiftUI or UIKit

## See Also

### Controlling Playback

func next()

Plays the next media item in the playlist.

Deprecated

func previous()

Plays the previous media item in the playlist.

Deprecated

var state: TVPlaybackState

The current state of the player.

Deprecated

enum TVPlaybackState

The possible states of a player.

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

