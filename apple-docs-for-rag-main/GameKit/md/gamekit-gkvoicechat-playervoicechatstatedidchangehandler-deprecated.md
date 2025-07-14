

- GameKit
- GKVoiceChat
-  playerVoiceChatStateDidChangeHandler Deprecated

Instance Property

# playerVoiceChatStateDidChangeHandler

A method that handles when a player’s voice chat changes state.

iOS 8.0–18.0DeprecatediPadOS 8.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.10–15.0DeprecatedtvOS 9.0–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
var playerVoiceChatStateDidChangeHandler: (GKPlayer, GKVoiceChat.PlayerState) -> Void { get set }
```

Deprecated

No longer supported

## Mentioned in 

Adding voice chat to multiplayer games

## Discussion

Set this property to update your interface when the state of any player in the chat changes, including the local player. For example, update the names or avatars when the players are connecting, speaking, or disconnecting.

The handler receives the following parameters:

`player`  
The player whose status changed.

`state`  
The new state of the player.

## See Also

### Receiving Updates About Other Participants

enum PlayerState

The state of a player in a voice chat.

Deprecated

