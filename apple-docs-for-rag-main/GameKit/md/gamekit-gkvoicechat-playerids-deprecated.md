

- GameKit
- GKVoiceChat
-  playerIDs Deprecated

Instance Property

# playerIDs

An array of strings containing the player identifiers for the players connected to the channel.

iOS 5.0–8.0DeprecatediPadOS 5.0–8.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.8–10.10DeprecatedvisionOS 1.0–1.0Deprecated

``` source
var playerIDs: [String]? { get }
```

Deprecated

Use the players property instead.

## See Also

### Deprecated Methods and Properties

var playerStateUpdateHandler: (String, GKVoiceChat.PlayerState) -> Void

Handles when a player in the chat changes state.

Deprecated

func setMute(Bool, forPlayer: String)

Mutes a player in a voice chat.

Deprecated

