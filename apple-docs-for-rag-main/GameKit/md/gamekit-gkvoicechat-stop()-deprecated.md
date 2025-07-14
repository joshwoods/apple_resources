

- GameKit
- GKVoiceChat
-  stop() Deprecated

Instance Method

# stop()

Ends communication with other players in a channel.

iOS 4.1–18.0DeprecatediPadOS 4.1–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.8–15.0DeprecatedtvOS 9.0–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
func stop()
```

Deprecated

No longer supported

## Mentioned in 

Adding voice chat to multiplayer games

## Discussion

This method disconnects the player from the channel. You should call `stop()` before you set the voice chat object to `nil`.

## See Also

### Related Documentation

var playerStateUpdateHandler: (String, GKVoiceChat.PlayerState) -> Void

Handles when a player in the chat changes state.

Deprecated

### Starting and Stopping Voice Chat

func start()

Starts communication with other players in a channel.

Deprecated

var isActive: Bool

A Boolean value that indicates whether the channel is sampling the microphone.

Deprecated

