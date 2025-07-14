

- GameKit
- GKMatchmakerViewController
-  matchmakingMode 

Instance Property

# matchmakingMode

The mode that a multiplayer game uses to find players.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
@MainActor
var matchmakingMode: GKMatchmakingMode { get set }
```

## Mentioned in 

Finding multiple players for a game

## Discussion

This method throws an exception if the mode isn’t possible due to restrictions.

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

enum GKMatchmakingMode

Possible modes that a multiplayer game uses to find matches.

