

- TVMLKit
- TVPlayer
-  dispatch(event:userInfo:completion:) Deprecated

Instance Method

# dispatch(event:userInfo:completion:)

Dispatches custom playback events to the JavaScript environment.

tvOS 12.0–18.0Deprecated

``` source
func dispatch(
    event: TVPlaybackEvent,
    userInfo: (any TVPlaybackEventMarshaling)?,
    completion: ((Bool) -> Void)? = nil
)
```

``` source
func dispatch(
    event: TVPlaybackEvent,
    userInfo: (any TVPlaybackEventMarshaling)?
) async -> Bool
```

Deprecated

Please use SwiftUI or UIKit

## Parameters 

`event`  

The custom playback event to be dispatched.

`userInfo`  

The user information for the custom event.

`completion`  

A block that is called after the event has been dispatched. Contains the information required to process the event’s results.

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func dispatch(event: TVPlaybackEvent, userInfo: (any TVPlaybackEventMarshaling)?) async -> Bool
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

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

struct TVPlaybackEvent

Extend this structure to send your custom playback events to the JavaScript environment.

Deprecated

protocol TVPlaybackEventMarshaling

A protocol used for sending and receiving information across the JavaScript bridge.

Deprecated

class TVPlaybackCustomEventUserInfo

The user information used in a custom playback event.

Deprecated

