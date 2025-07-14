

- GameKit
- GKVoiceChat
-  playerStateUpdateHandler Deprecated

Instance Property

# playerStateUpdateHandler

Handles when a player in the chat changes state.

iOS 4.1–8.0DeprecatediPadOS 4.1–8.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.8–10.10DeprecatedvisionOS 1.0–1.0Deprecated

``` source
var playerStateUpdateHandler: (String, GKVoiceChat.PlayerState) -> Void { get set }
```

Deprecated

Use the setPlayer(_:muted:) method instead.

## Discussion

Your game sets this property with a block that GameKit calls when the state of any participant in the chat changes (including the local player). The block receives the following parameters:

`playerID`  
The player identifier for the player whose status changed.

`state`  
The new state of the player. See GKVoiceChat.PlayerState.

## See Also

### Deprecated Methods and Properties

var playerIDs: [String]?

An array of strings containing the player identifiers for the players connected to the channel.

Deprecated

func setMute(Bool, forPlayer: String)

Mutes a player in a voice chat.

Deprecated

