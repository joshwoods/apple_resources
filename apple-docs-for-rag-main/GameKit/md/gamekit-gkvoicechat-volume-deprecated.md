

- GameKit
- GKVoiceChat
-  volume Deprecated

Instance Property

# volume

The volume level for the channel.

iOS 4.1–18.0DeprecatediPadOS 4.1–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.8–15.0DeprecatedtvOS 9.0–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
var volume: Float { get set }
```

Deprecated

No longer supported

## Mentioned in 

Adding voice chat to multiplayer games

## Discussion

GameKit mixes voice data received from all other players and scales it by the `volume` property. The `volume` property has a range between `0.0` and `1.0`, inclusive. To mute the entire channel, set the volume to `0.0`. To play the voice data at full volume, set the volume to `1.0`. The default value is `1.0`.

## See Also

### Controlling Chat Volume

func setPlayer(GKPlayer, muted: Bool)

Mutes a player in the chat, including the local player.

Deprecated

