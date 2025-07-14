

- GameKit
- GKGameCenterViewController
-  init(leaderboardID:playerScope:timeScope:) 

Initializer

# init(leaderboardID:playerScope:timeScope:)

Creates a view controller that presents a leaderboard with data from the specified players and time period.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
@MainActor
init(
    leaderboardID: String,
    playerScope: GKLeaderboard.PlayerScope,
    timeScope: GKLeaderboard.TimeScope
)
```

## Parameters 

`leaderboardID`  

The identifier for the leaderboard to display.

`playerScope`  

The type of players to display in the leaderboard.

`timeScope`  

The time period for the data to display in a classic leaderboard.

For recurring leaderboards, this method ignores the time scope parameter and displays the data for the current occurrence instead.

## Return Value

The initialized view controller.

## See Also

### Configuring Game Center content

init(state: GKGameCenterViewControllerState)

Creates a view controller that presents the specified Game Center content.

enum GKGameCenterViewControllerState

The type of content for the view controller to present.

init(leaderboard: GKLeaderboard, playerScope: GKLeaderboard.PlayerScope)

Creates a view controller that presents a leaderboard with data for the specified players.

init(leaderboardSetID: String)

Creates a view controller that presents a leaderboard set.

init(achievementID: String)

Creates a view controller that presents an achievement.

init(player: GKPlayer)

Creates a view controller that presents a player’s Game Center profile.

