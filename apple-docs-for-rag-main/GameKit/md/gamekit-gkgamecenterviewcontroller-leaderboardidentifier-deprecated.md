

- GameKit
- GKGameCenterViewController
-  leaderboardIdentifier Deprecated

Instance Property

# leaderboardIdentifier

The named leaderboard that the view controller displays.

iOS 7.0–14.0DeprecatediPadOS 7.0–14.0DeprecatedMac Catalyst 13.1–14.0DeprecatedmacOS 10.10–11.0DeprecatedtvOS 9.0–14.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
@MainActor
var leaderboardIdentifier: String? { get set }
```

Deprecated

Use init(leaderboard:playerScope:) instead.

## Discussion

The leaderboardIdentifier property must either be `nil` or it must match a leaderboard identifier you defined when you created your leaderboards in App Store Connect. If `nil`, the view displays scores for the aggregate leaderboard. Default is `nil`.

When the leaderboard is presented, the value of this property determines which leaderboard content is displayed to the player. As the player changes which leaderboard content they view, the leaderboardIdentifier property is automatically updated. For example, to preserve the player’s selections, you can read the leaderboardIdentifier property after the screen is dismissed, and set that value the next time you initialize the view controller.

## See Also

### Deprecated Properties

var viewState: GKGameCenterViewControllerState

The content that the Game Center controller displays.

Deprecated

var leaderboardCategory: String?

The named leaderboard that the view controller displays.

Deprecated

var leaderboardTimeScope: GKLeaderboard.TimeScope

A time filter that restricts the scores to display to the player.

Deprecated

