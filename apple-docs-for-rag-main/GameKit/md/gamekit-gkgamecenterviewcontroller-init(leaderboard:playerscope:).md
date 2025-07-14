

- GameKit
- GKGameCenterViewController
-  init(leaderboard:playerScope:) 

Initializer

# init(leaderboard:playerScope:)

Creates a view controller that presents a leaderboard with data for the specified players.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
@MainActor
init(
    leaderboard: GKLeaderboard,
    playerScope: GKLeaderboard.PlayerScope
)
```

## Parameters 

`leaderboard`  

The identifier for the leaderboard to display.

`playerScope`  

The type of players to display in the leaderboard.

## Return Value

The initialized view controller.

## See Also

### Configuring Game Center content

init(state: GKGameCenterViewControllerState)

Creates a view controller that presents the specified Game Center content.

enum GKGameCenterViewControllerState

The type of content for the view controller to present.

init(leaderboardID: String, playerScope: GKLeaderboard.PlayerScope, timeScope: GKLeaderboard.TimeScope)

Creates a view controller that presents a leaderboard with data from the specified players and time period.

init(leaderboardSetID: String)

Creates a view controller that presents a leaderboard set.

init(achievementID: String)

Creates a view controller that presents an achievement.

init(player: GKPlayer)

Creates a view controller that presents a player’s Game Center profile.

