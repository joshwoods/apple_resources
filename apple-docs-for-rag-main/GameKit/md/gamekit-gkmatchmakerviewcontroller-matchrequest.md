

- GameKit
- GKMatchmakerViewController
-  matchRequest 

Instance Property

# matchRequest

The configuration for the desired match.

iOS 4.1+iPadOS 4.1+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
var matchRequest: GKMatchRequest { get }
```

## See Also

### Creating and configuring the view controller

init?(matchRequest: GKMatchRequest)

Creates a matchmaker view controller for the local player to start inviting other players.

init?(invite: GKInvite)

Creates a matchmaker view controller to present to a player who accepts an invitation.

var canStartWithMinimumPlayers: Bool

A Boolean value that indicates whether your game can start after a minimum number of players join a match.

var matchmakingMode: GKMatchmakingMode

The mode that a multiplayer game uses to find players.

enum GKMatchmakingMode

Possible modes that a multiplayer game uses to find matches.

