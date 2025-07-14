

- GameKit
- GKAccessPoint
-  trigger(handler:) 

Instance Method

# trigger(handler:)

Displays the Game Center dashboard as if the player taps or presses the access point.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
func trigger(handler: @escaping () -> Void)
```

## Parameters 

`handler`  

The block that GameKit calls after it displays the dashboard.

## Discussion

For games that use controllers or the Apple TV remote, you can use this method to programmatically display the dashboard.

## See Also

### Managing the access point

var isFocused: Bool

A Boolean value that indicates whether the access point is in focus on tvOS.

func trigger(state: GKGameCenterViewControllerState, handler: () -> Void)

Displays the Game Center dashboard in the specified state as if the player taps or presses the access point.

func trigger(player: GKPlayer, handler: (() -> Void)?)

Displays the Game Center dashboard in a state that shows a player profile.

func trigger(achievementID: String, handler: (() -> Void)?)

Displays the Game Center dashboard in a state that shows a specific achievement.

func trigger(leaderboardID: String, playerScope: GKLeaderboard.PlayerScope, timeScope: GKLeaderboard.TimeScope, handler: (() -> Void)?)

Displays the Game Center dashboard in a state that shows a specific leaderboard.

func trigger(leaderboardSetID: String, handler: (() -> Void)?)

Displays the Game Center dashboard in a state that shows a specific leaderboard set.

