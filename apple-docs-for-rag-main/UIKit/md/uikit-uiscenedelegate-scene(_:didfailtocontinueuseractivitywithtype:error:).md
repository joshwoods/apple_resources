

- UIKit
- UISceneDelegate
-  scene(\_:didFailToContinueUserActivityWithType:error:) 

Instance Method

# scene(\_:didFailToContinueUserActivityWithType:error:)

Tells the delegate that the activity couldn’t be continued.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
optional func scene(
    _ scene: UIScene,
    didFailToContinueUserActivityWithType userActivityType: String,
    error: any Error
)
```

## Parameters 

`scene`  

The scene handling the activity.

`userActivityType`  

The type of the activity that failed.

`error`  

An error object indicating the reason for the failure.

## Discussion

Use this method to let the user know that the specified activity couldn’t be completed. If you don’t implement this method, UIKit displays an error to the user with an appropriate message about the reason for the failure.

## See Also

### Continuing user activities

func scene(UIScene, willContinueUserActivityWithType: String)

Tells the delegate that it’s about to receive Handoff-related data.

func scene(UIScene, continue: NSUserActivity)

Tells the delegate to handle the specified Handoff-related activity.

