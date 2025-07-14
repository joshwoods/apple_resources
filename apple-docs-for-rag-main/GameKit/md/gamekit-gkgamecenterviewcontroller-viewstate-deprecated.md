

- GameKit
- GKGameCenterViewController
-  viewState Deprecated

Instance Property

# viewState

The content that the Game Center controller displays.

iOS 6.0–14.0DeprecatediPadOS 6.0–14.0DeprecatedMac Catalyst 13.1–14.0DeprecatedmacOS 10.9–11.0DeprecatedtvOS 9.0–14.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
@MainActor
var viewState: GKGameCenterViewControllerState { get set }
```

Deprecated

Use init(state:) instead.

## Discussion

See GKGameCenterViewControllerState for possible values. When you first present the Game Center view controller, the content displayed by the view controller is determined by this property. If the player navigates to different content, the view state is automatically updated. For example, to preserve the player’s selections, you can read the viewState property after the screen is dismissed, and set that value the next time you initialize the view controller.

## See Also

### Deprecated Properties

var leaderboardIdentifier: String?

The named leaderboard that the view controller displays.

Deprecated

var leaderboardCategory: String?

The named leaderboard that the view controller displays.

Deprecated

var leaderboardTimeScope: GKLeaderboard.TimeScope

A time filter that restricts the scores to display to the player.

Deprecated

