

- GameKit
- GKTurnBasedMatchmakerViewController
-  init(matchRequest:) 

Initializer

# init(matchRequest:)

Creates a matchmaker view controller for the local player to start inviting other players to a turn-based game.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
@MainActor
init(matchRequest request: GKMatchRequest)
```

## Parameters 

`request`  

A match request that you configure for the characteristics of your game.

## Return Value

An initialized matchmaker view controller object or `nil` If an error occurs.

## See Also

### Creating and Configuring the View Controller

var showExistingMatches: Bool

A Boolean value that determines whether the view controller shows existing matches.

var matchmakingMode: GKMatchmakingMode

The mode that a multiplayer game uses to find players.

enum GKMatchmakingMode

Possible modes that a multiplayer game uses to find matches.

