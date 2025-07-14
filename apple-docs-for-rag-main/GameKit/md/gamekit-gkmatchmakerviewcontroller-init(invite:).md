

- GameKit
- GKMatchmakerViewController
-  init(invite:) 

Initializer

# init(invite:)

Creates a matchmaker view controller to present to a player who accepts an invitation.

iOS 4.1+iPadOS 4.1+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
init?(invite: GKInvite)
```

## Parameters 

`invite`  

The invitation that the player accepts.

## Return Value

An initialized matchmaker view controller object. If an error occurs, returns `nil`.

## Discussion

The interface shows the status of the other players accepting and declining their invitations until the game starts.

## See Also

### Creating and configuring the view controller

init?(matchRequest: GKMatchRequest)

Creates a matchmaker view controller for the local player to start inviting other players.

var matchRequest: GKMatchRequest

The configuration for the desired match.

var canStartWithMinimumPlayers: Bool

A Boolean value that indicates whether your game can start after a minimum number of players join a match.

var matchmakingMode: GKMatchmakingMode

The mode that a multiplayer game uses to find players.

enum GKMatchmakingMode

Possible modes that a multiplayer game uses to find matches.

