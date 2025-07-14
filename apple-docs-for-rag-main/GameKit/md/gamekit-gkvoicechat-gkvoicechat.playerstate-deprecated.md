

- GameKit
- GKVoiceChat
-  GKVoiceChat.PlayerState Deprecated

Enumeration

# GKVoiceChat.PlayerState

The state of a player in a voice chat.

iOS 4.1–18.0DeprecatediPadOS 4.1–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.8–15.0DeprecatedtvOS 9.0–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
enum PlayerState
```

Deprecated

Use SharePlay instead. See Enable the local player to choose other players and startGroupActivity(playerHandler:).

## Topics

### States

case connected

The state when the player connects to the channel.

case disconnected

The state when the player left the channel.

case speaking

The state when the player speaks.

case silent

The state when the player isn’t speaking.

case connecting

The state when the player is connecting to the channel, but isn’t connected yet.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Receiving Updates About Other Participants

var playerVoiceChatStateDidChangeHandler: (GKPlayer, GKVoiceChat.PlayerState) -> Void

A method that handles when a player’s voice chat changes state.

Deprecated

