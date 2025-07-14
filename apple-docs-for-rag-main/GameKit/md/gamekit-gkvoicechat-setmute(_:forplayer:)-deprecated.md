

- GameKit
- GKVoiceChat
-  setMute(\_:forPlayer:) Deprecated

Instance Method

# setMute(\_:forPlayer:)

Mutes a player in a voice chat.

iOS 5.0–8.0DeprecatediPadOS 5.0–8.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.8–10.10DeprecatedvisionOS 1.0–1.0Deprecated

``` source
func setMute(
    _ isMuted: Bool,
    forPlayer playerID: String
)
```

Deprecated

Use the setPlayer(_:muted:) method instead.

## Parameters 

`isMuted`  

Determines whether to mute or unmute the player.

`playerID`  

The player identifier string for a player in the match.

## Discussion

If you mute a player, the local player doesn’t hear voice data transmitted by that player.

## See Also

### Deprecated Methods and Properties

var playerIDs: [String]?

An array of strings containing the player identifiers for the players connected to the channel.

Deprecated

var playerStateUpdateHandler: (String, GKVoiceChat.PlayerState) -> Void

Handles when a player in the chat changes state.

Deprecated

