

- GameKit
- GKLeaderboardViewController
-  timeScope 

Instance Property

# timeScope

A time filter used to restrict which scores are displayed to the player.

macOSvisionOS

``` source
@MainActor
var timeScope: GKLeaderboard.TimeScope { get set }
```

## Discussion

This property determines which tab view is displayed to the player. The default value is GKLeaderboard.TimeScope.allTime, which shows the best score each player has earned. For more information on time scopes, see GKLeaderboard.

If the player changes which tab they view, the `timeScope` property is automatically updated. For example, you can read the `timeScope` property after the view controller is dismissed, and set that value the next time you initialize a new leaderboard view controller.

## See Also

### Configuring the Leaderboard View Controller

var category: String!

The named leaderboard that is displayed by the view controller.

var leaderboardDelegate: (any GKLeaderboardViewControllerDelegate)!

The view controller’s delegate.

