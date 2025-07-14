

- UIKit
- UISceneDelegate
-  stateRestorationActivity(for:) 

Instance Method

# stateRestorationActivity(for:)

Returns a user activity object encapsulating the current state of the specified scene.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
optional func stateRestorationActivity(for scene: UIScene) -> NSUserActivity?
```

## Parameters 

`scene`  

The scene whose state information is needed.

## Discussion

Use this method to return an NSUserActivity object with information about your scene’s current state. Save enough information to be able to restore that state again after UIKit disconnects and then reconnects the scene. User activity objects are a mechanism to record what the user is doing, so you don’t need to manually persist the state of your scene’s UI.

After calling this method, and before archiving the NSUserActivity object and saving it to disk, UIKit lets you add state information as follows:

- If you set a delegate for the NSUserActivity object in your app, UIKit calls the delegate’s userActivityWillSave(_:) method.

- If you assign the NSUserActivity object to the userActivity property of any responders, UIKit calls each responder’s updateUserActivityState(_:) method.

When reconnecting the scene and restoring state, the user activity provided by this method will be provided in the stateRestorationActivity property of UISceneSession.

## See Also

### Saving the state of the scene

Restoring your app’s state

Provide continuity for the user by preserving current activities.

func scene(UIScene, restoreInteractionStateWith: NSUserActivity)

func scene(UIScene, didUpdate: NSUserActivity)

Tells the delegate that the specified activity object was updated.

