

- UIKit
- UISceneDelegate
-  scene(\_:restoreInteractionStateWith:) 

Instance Method

# scene(\_:restoreInteractionStateWith:)

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
optional func scene(
    _ scene: UIScene,
    restoreInteractionStateWith stateRestorationActivity: NSUserActivity
)
```

## See Also

### Saving the state of the scene

Restoring your app’s state

Provide continuity for the user by preserving current activities.

func stateRestorationActivity(for: UIScene) -> NSUserActivity?

Returns a user activity object encapsulating the current state of the specified scene.

func scene(UIScene, didUpdate: NSUserActivity)

Tells the delegate that the specified activity object was updated.

