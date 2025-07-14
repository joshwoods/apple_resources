

- GameKit
- GKAccessPoint
-  trigger(leaderboardID:playerScope:timeScope:handler:) 

Instance Method

# trigger(leaderboardID:playerScope:timeScope:handler:)

Displays the Game Center dashboard in a state that shows a specific leaderboard.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
func trigger(
    leaderboardID: String,
    playerScope: GKLeaderboard.PlayerScope,
    timeScope: GKLeaderboard.TimeScope,
    handler: (() -> Void)? = nil
)
```

## Parameters 

`leaderboardID`  

The identifier for the leaderboard.

`playerScope`  

The type of players for scoping the leaderboard data.

`timeScope`  

The time period for filtering the leaderboard data.

`handler`  

The block that GameKit calls after it displays the dashboard.

## See Also

### Managing the access point

var isFocused: Bool

A Boolean value that indicates whether the access point is in focus on tvOS.

func trigger(handler: () -> Void)

Displays the Game Center dashboard as if the player taps or presses the access point.

func trigger(state: GKGameCenterViewControllerState, handler: () -> Void)

Displays the Game Center dashboard in the specified state as if the player taps or presses the access point.

func trigger(player: GKPlayer, handler: (() -> Void)?)

Displays the Game Center dashboard in a state that shows a player profile.

func trigger(achievementID: String, handler: (() -> Void)?)

Displays the Game Center dashboard in a state that shows a specific achievement.

func trigger(leaderboardSetID: String, handler: (() -> Void)?)

Displays the Game Center dashboard in a state that shows a specific leaderboard set.

