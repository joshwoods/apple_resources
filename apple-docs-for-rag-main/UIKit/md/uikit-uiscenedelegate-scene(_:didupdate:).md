

- UIKit
- UISceneDelegate
-  scene(\_:didUpdate:) 

Instance Method

# scene(\_:didUpdate:)

Tells the delegate that the specified activity object was updated.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
optional func scene(
    _ scene: UIScene,
    didUpdate userActivity: NSUserActivity
)
```

## Parameters 

`scene`  

The scene handling the activity.

`userActivity`  

The user activity object containing the updated data.

## Discussion

Use this method to add any final data to the specified user activity object. UIKit calls this method on your app’s main thread after calling your stateRestorationActivity(for:) method and after giving other parts of your app an opportunity to update the activity object returned by that method.

## See Also

### Saving the state of the scene

Restoring your app’s state

Provide continuity for the user by preserving current activities.

func stateRestorationActivity(for: UIScene) -> NSUserActivity?

Returns a user activity object encapsulating the current state of the specified scene.

func scene(UIScene, restoreInteractionStateWith: NSUserActivity)

