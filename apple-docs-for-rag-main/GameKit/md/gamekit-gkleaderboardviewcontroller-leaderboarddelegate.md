

- GameKit
- GKLeaderboardViewController
-  leaderboardDelegate 

Instance Property

# leaderboardDelegate

The view controller’s delegate.

macOSvisionOS

``` source
@MainActor
weak var leaderboardDelegate: (any GKLeaderboardViewControllerDelegate)! { get set }
```

## Discussion

Before displaying the leaderboard, you must set a delegate.

## See Also

### Configuring the Leaderboard View Controller

var category: String!

The named leaderboard that is displayed by the view controller.

var timeScope: GKLeaderboard.TimeScope

A time filter used to restrict which scores are displayed to the player.

