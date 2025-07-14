

- GameKit
- GKVoiceChat
-  setPlayer(\_:muted:) Deprecated

Instance Method

# setPlayer(\_:muted:)

Mutes a player in the chat, including the local player.

iOS 8.0–18.0DeprecatediPadOS 8.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.10–15.0DeprecatedtvOS 9.0–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
func setPlayer(
    _ player: GKPlayer,
    muted isMuted: Bool
)
```

Deprecated

No longer supported

## Parameters 

`player`  

The player that GameKit mutes or unmutes.

`isMuted`  

Determines whether to mute or unmute the player.

## Mentioned in 

Adding voice chat to multiplayer games

## Discussion

If you mute another player, the local player doesn’t hear voice data from that player.

## See Also

### Controlling Chat Volume

var volume: Float

The volume level for the channel.

Deprecated

