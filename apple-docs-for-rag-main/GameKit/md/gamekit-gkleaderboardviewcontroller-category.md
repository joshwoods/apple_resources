

- GameKit
- GKLeaderboardViewController
-  category 

Instance Property

# category

The named leaderboard that is displayed by the view controller.

macOSvisionOS

``` source
@MainActor
var category: String! { get set }
```

## Discussion

The `category` property must either be `nil` or it must match a leaderboard identifier for a leaderboard you defined in App Store Connect. If `nil`, the view displays scores for the default leaderboard. Default is `nil`.

When the view controller is presented, the initial leaderboard shown is based on the value of this property. If the player changes which leaderboard they are viewing, the `category` property is automatically updated. For example, you can read the `category` property after the screen is dismissed, and set that value the next time you initialize a new leaderboard view controller.

## See Also

### Configuring the Leaderboard View Controller

var leaderboardDelegate: (any GKLeaderboardViewControllerDelegate)!

The view controller’s delegate.

var timeScope: GKLeaderboard.TimeScope

A time filter used to restrict which scores are displayed to the player.

