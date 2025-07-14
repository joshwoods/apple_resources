

- GameKit
- GKVoiceChat
-  start() Deprecated

Instance Method

# start()

Starts communication with other players in a channel.

iOS 4.1–18.0DeprecatediPadOS 4.1–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.8–15.0DeprecatedtvOS 9.0–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
func start()
```

Deprecated

No longer supported

## Mentioned in 

Adding voice chat to multiplayer games

## Discussion

You must provide a reason, by adding the NSMicrophoneUsageDescription key to the Information Property List, to start voice chat with other players.

If the player grants permission to use the microphone and this method successfully connects to the channel, GameKit plays voice data from the other players automatically. Use the isActive property to begin sending the local player’s microphone data to the channel.

A player can only start voice chat if their device has a microphone and they connect to Wi-Fi.

## See Also

### Starting and Stopping Voice Chat

func stop()

Ends communication with other players in a channel.

Deprecated

var isActive: Bool

A Boolean value that indicates whether the channel is sampling the microphone.

Deprecated

