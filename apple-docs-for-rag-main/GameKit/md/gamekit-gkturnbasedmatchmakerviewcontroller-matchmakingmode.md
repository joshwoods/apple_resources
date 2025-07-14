

- GameKit
- GKTurnBasedMatchmakerViewController
-  matchmakingMode 

Instance Property

# matchmakingMode

The mode that a multiplayer game uses to find players.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
@MainActor
var matchmakingMode: GKMatchmakingMode { get set }
```

## Mentioned in 

Starting turn-based matches and passing turns between players

## Discussion

This method throws an exception if you set the mode to a value that isn’t possible due to restrictions.

## See Also

### Creating and Configuring the View Controller

init(matchRequest: GKMatchRequest)

Creates a matchmaker view controller for the local player to start inviting other players to a turn-based game.

var showExistingMatches: Bool

A Boolean value that determines whether the view controller shows existing matches.

enum GKMatchmakingMode

Possible modes that a multiplayer game uses to find matches.

