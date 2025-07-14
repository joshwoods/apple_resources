

- UIKit
- UISceneDelegate
-  scene(\_:continue:) 

Instance Method

# scene(\_:continue:)

Tells the delegate to handle the specified Handoff-related activity.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
optional func scene(
    _ scene: UIScene,
    continue userActivity: NSUserActivity
)
```

## Parameters 

`scene`  

The scene handling the activity.

`userActivity`  

The object containing the activity-related data. Use the information in this object to continue the user’s activity in your scene.

## Discussion

Use this method to update the specified scene with the data from the provided activity object. UIKit calls this method on your app’s main thread only after it receives all of the data for an activity object, which might originate from a different device.

## See Also

### Continuing user activities

func scene(UIScene, willContinueUserActivityWithType: String)

Tells the delegate that it’s about to receive Handoff-related data.

func scene(UIScene, didFailToContinueUserActivityWithType: String, error: any Error)

Tells the delegate that the activity couldn’t be continued.

