

- TVMLKit
-  TVPlaybackCustomEventUserInfo Deprecated

Class

# TVPlaybackCustomEventUserInfo

The user information used in a custom playback event.

tvOS 12.0–18.0Deprecated

``` source
class TVPlaybackCustomEventUserInfo
```

Deprecated

Please use SwiftUI or UIKit

## Topics

### Creating User Info for Custom Playback Events

init(properties: [TVPlaybackEventProperty : Any]?, expectsReturnValue: Bool)

Create a new custom playback event user info dictionary.

struct TVPlaybackEventProperty

Extend this structure to create your own custom playback event properties.

var expectsReturnValue: Bool

A Boolean value that indicates whether the custom event expects to contain a return value.

var returnValue: Any?

The return value type for the custom event.

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
- TVPlaybackEventMarshaling

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

