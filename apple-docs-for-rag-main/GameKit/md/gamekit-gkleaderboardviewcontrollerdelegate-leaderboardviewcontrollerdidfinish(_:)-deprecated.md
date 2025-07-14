

- GameKit
- GKLeaderboardViewControllerDelegate
-  leaderboardViewControllerDidFinish(\_:) Deprecated

Instance Method

# leaderboardViewControllerDidFinish(\_:)

Called when the leaderboard view is dismissed.

macOS 10.8–10.10DeprecatedvisionOS 1.0–1.0Deprecated

``` source
func leaderboardViewControllerDidFinish(_ viewController: GKLeaderboardViewController!)
```

**Required**

## Parameters 

`viewController`  

The leaderboard view controller that was dismissed by the player.

## Discussion

Your delegate should dismiss the view controller. If your game paused any gameplay or other activities, it can restart those services in this method.

