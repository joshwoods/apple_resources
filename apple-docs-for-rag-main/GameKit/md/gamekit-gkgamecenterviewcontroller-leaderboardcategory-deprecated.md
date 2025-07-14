

- GameKit
- GKGameCenterViewController
-  leaderboardCategory Deprecated

Instance Property

# leaderboardCategory

The named leaderboard that the view controller displays.

macOS 10.8–10.10DeprecatedvisionOS 1.0–1.0Deprecated

``` source
@MainActor
var leaderboardCategory: String? { get set }
```

Deprecated

Use init(leaderboard:playerScope:) instead.

## Discussion

The category property must either be `nil` or it must match a category identifier you defined when you created your leaderboards in App Store Connect. If `nil`, the view displays scores for the aggregate leaderboard. Default is `nil`.

When the leaderboard is presented, the value of this property determines which leaderboard content is displayed to the player. As the player changes which leaderboard content they view, the leaderboardCategory property is automatically updated. For example, to preserve the player’s selections, you can read the leaderboardCategory property after the screen is dismissed, and set that value the next time you initialize the view controller.

## See Also

### Deprecated Properties

var viewState: GKGameCenterViewControllerState

The content that the Game Center controller displays.

Deprecated

var leaderboardIdentifier: String?

The named leaderboard that the view controller displays.

Deprecated

var leaderboardTimeScope: GKLeaderboard.TimeScope

A time filter that restricts the scores to display to the player.

Deprecated

