

- GameKit
- GKGameCenterViewController
-  init(achievementID:) 

Initializer

# init(achievementID:)

Creates a view controller that presents an achievement.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
@MainActor
init(achievementID: String)
```

## Parameters 

`achievementID`  

The identifier for the achievement to display.

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

init(leaderboardID: String, playerScope: GKLeaderboard.PlayerScope, timeScope: GKLeaderboard.TimeScope)

Creates a view controller that presents a leaderboard with data from the specified players and time period.

init(leaderboardSetID: String)

Creates a view controller that presents a leaderboard set.

init(player: GKPlayer)

Creates a view controller that presents a player’s Game Center profile.

