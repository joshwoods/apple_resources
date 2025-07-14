

- GameKit
- GKGameCenterViewController
-  leaderboardTimeScope Deprecated

Instance Property

# leaderboardTimeScope

A time filter that restricts the scores to display to the player.

iOS 4.1–14.0DeprecatediPadOS 4.1–14.0DeprecatedMac Catalyst 13.1–14.0DeprecatedmacOS 10.8–11.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
@MainActor
var leaderboardTimeScope: GKLeaderboard.TimeScope { get set }
```

Deprecated

Use init(leaderboardID:playerScope:timeScope:) instead.

## Discussion

This property determines which tab view of the scores screen is displayed to the player. The default value is GKLeaderboard.TimeScope.allTime, which shows the best score each player has earned. For more information on time scopes, see GKLeaderboard.

When the leaderboard is presented, the value of this property determines the initial tab that is displayed to the player. As the player changes which tab they view, the leaderboardTimeScope property is automatically updated. For example, to preserve the player’s selections, you can read the leaderboardTimeScope property after the screen is dismissed, and set that value the next time you initialize the view controller.

## See Also

### Deprecated Properties

var viewState: GKGameCenterViewControllerState

The content that the Game Center controller displays.

Deprecated

var leaderboardIdentifier: String?

The named leaderboard that the view controller displays.

Deprecated

var leaderboardCategory: String?

The named leaderboard that the view controller displays.

Deprecated

