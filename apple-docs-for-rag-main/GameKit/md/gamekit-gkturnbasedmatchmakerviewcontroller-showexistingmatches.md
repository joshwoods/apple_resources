

- GameKit
- GKTurnBasedMatchmakerViewController
-  showExistingMatches 

Instance Property

# showExistingMatches

A Boolean value that determines whether the view controller shows existing matches.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
@MainActor
var showExistingMatches: Bool { get set }
```

## Mentioned in 

Starting turn-based matches and passing turns between players

## Discussion

If the value of this property is true, the view controller shows matches that are in progress or complete. If the value of this property is false, the view controller only offers the ability to create new matches. The default value is true.

## See Also

### Creating and Configuring the View Controller

init(matchRequest: GKMatchRequest)

Creates a matchmaker view controller for the local player to start inviting other players to a turn-based game.

var matchmakingMode: GKMatchmakingMode

The mode that a multiplayer game uses to find players.

enum GKMatchmakingMode

Possible modes that a multiplayer game uses to find matches.

