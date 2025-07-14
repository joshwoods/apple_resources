

- UIKit
- UISceneDelegate
-  scene(\_:willContinueUserActivityWithType:) 

Instance Method

# scene(\_:willContinueUserActivityWithType:)

Tells the delegate that it’s about to receive Handoff-related data.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
optional func scene(
    _ scene: UIScene,
    willContinueUserActivityWithType userActivityType: String
)
```

## Parameters 

`scene`  

The scene handling the activity.

`userActivityType`  

The type of activity to continue.

## Discussion

Use this method to prepare to handle an activity with the specified type. After this method returns, UIKit provides feedback to the user that your scene is handling the activity.

## See Also

### Continuing user activities

func scene(UIScene, continue: NSUserActivity)

Tells the delegate to handle the specified Handoff-related activity.

func scene(UIScene, didFailToContinueUserActivityWithType: String, error: any Error)

Tells the delegate that the activity couldn’t be continued.

