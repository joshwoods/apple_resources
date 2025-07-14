

- GameKit
- GKAchievementViewControllerDelegate
-  achievementViewControllerDidFinish(\_:) Deprecated

Instance Method

# achievementViewControllerDidFinish(\_:)

Called when the user dismisses the achievements user interface.

macOS 10.8–10.10DeprecatedvisionOS 1.0–1.0Deprecated

``` source
func achievementViewControllerDidFinish(_ viewController: GKAchievementViewController!)
```

**Required**

## Parameters 

`viewController`  

The achievement view controller whose interface was dismissed by the player.

## Discussion

Your delegate should dismiss the view controller. If your game paused any gameplay or other activities, it can restart those services in this method.

