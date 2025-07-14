

- GameKit
-  GKGameCenterViewControllerState 

Enumeration

# GKGameCenterViewControllerState

The type of content for the view controller to present.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+

``` source
enum GKGameCenterViewControllerState
```

## Topics

### States

case `default`

The view controller should present the default screen.

case leaderboards

The view controller should present leaderboard sets or leaderboards if there are no sets.

case achievements

The view controller should present a list of achievements.

case challenges

The view controller should present a list of challenges.

case localPlayerProfile

The view controller should present the local player’s profile.

case dashboard

The view controller should present the dashboard.

case localPlayerFriendsList

The view controller should present the friends list.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Configuring Game Center content

init(state: GKGameCenterViewControllerState)

Creates a view controller that presents the specified Game Center content.

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

