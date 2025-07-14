

- GameKit
-  GKMatchmakingMode 

Enumeration

# GKMatchmakingMode

Possible modes that a multiplayer game uses to find matches.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
enum GKMatchmakingMode
```

## Topics

### Modes

case `default`

The default matchmaking mode.

case nearbyOnly

A mode that matches the local player only with nearby players.

case automatchOnly

A mode that matches the local player only with players who are also actively looking for a match.

case inviteOnly

A mode that matches the local player only with players who they invite, and doesn’t use automatch to fill empty slots.

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

### Creating and configuring the view controller

init?(matchRequest: GKMatchRequest)

Creates a matchmaker view controller for the local player to start inviting other players.

init?(invite: GKInvite)

Creates a matchmaker view controller to present to a player who accepts an invitation.

var matchRequest: GKMatchRequest

The configuration for the desired match.

var canStartWithMinimumPlayers: Bool

A Boolean value that indicates whether your game can start after a minimum number of players join a match.

var matchmakingMode: GKMatchmakingMode

The mode that a multiplayer game uses to find players.

