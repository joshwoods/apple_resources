

- GameKit
- GKAccessPoint
-  isFocused 

Instance Property

# isFocused

A Boolean value that indicates whether the access point is in focus on tvOS.

tvOS 14.0+

``` source
var isFocused: Bool { get set }
```

## Discussion

To change the focus to the access point, set this property to true; otherwise, set it to false.

## See Also

### Managing the access point

func trigger(handler: () -> Void)

Displays the Game Center dashboard as if the player taps or presses the access point.

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

