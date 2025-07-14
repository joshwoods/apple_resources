

- GameKit
- GKGameCenterViewController
-  init(leaderboardSetID:) 

Initializer

# init(leaderboardSetID:)

Creates a view controller that presents a leaderboard set.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
@MainActor
init(leaderboardSetID: String)
```

## Parameters 

`leaderboardSetID`  

The identifier for the leaderboard set.

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

init(achievementID: String)

Creates a view controller that presents an achievement.

init(player: GKPlayer)

Creates a view controller that presents a player’s Game Center profile.

