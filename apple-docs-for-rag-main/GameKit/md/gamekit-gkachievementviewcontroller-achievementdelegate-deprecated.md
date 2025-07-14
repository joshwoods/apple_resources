

- GameKit
- GKAchievementViewController
-  achievementDelegate Deprecated

Instance Property

# achievementDelegate

The achievement view controller’s delegate.

macOS 10.8–10.10DeprecatedvisionOS 1.0–1.0Deprecated

``` source
@MainActor
weak var achievementDelegate: (any GKAchievementViewControllerDelegate)! { get set }
```

## Discussion

Your game must set the delegate before presenting the view controller.

