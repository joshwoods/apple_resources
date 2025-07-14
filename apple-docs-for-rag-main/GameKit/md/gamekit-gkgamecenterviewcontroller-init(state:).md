

- GameKit
- GKGameCenterViewController
-  init(state:) 

Initializer

# init(state:)

Creates a view controller that presents the specified Game Center content.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
@MainActor
init(state: GKGameCenterViewControllerState)
```

## Parameters 

`state`  

The type of content to present.

## Return Value

The initialized view controller.

## Mentioned in 

Displaying the Game Center dashboard

## See Also

### Configuring Game Center content

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

init(player: GKPlayer)

Creates a view controller that presents a player’s Game Center profile.

