

- GameKit
- GKGameCenterViewController
-  init(player:) 

Initializer

# init(player:)

Creates a view controller that presents a player’s Game Center profile.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
@MainActor
init(player: GKPlayer)
```

## Parameters 

`player`  

The player to show in the view controller.

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

init(achievementID: String)

Creates a view controller that presents an achievement.

