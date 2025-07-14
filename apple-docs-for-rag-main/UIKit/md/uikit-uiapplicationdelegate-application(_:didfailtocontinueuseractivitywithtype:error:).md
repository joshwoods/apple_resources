

- UIKit
- UIApplicationDelegate
-  application(\_:didFailToContinueUserActivityWithType:error:) 

Instance Method

# application(\_:didFailToContinueUserActivityWithType:error:)

Tells the delegate that the activity couldn’t be continued.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
optional func application(
    _ application: UIApplication,
    didFailToContinueUserActivityWithType userActivityType: String,
    error: any Error
)
```

## Parameters 

`application`  

Your shared app object.

`userActivityType`  

The activity type that was attempted.

`error`  

An error object indicating the reason for the failure.

## Discussion

Use this method to let the user know that the specified activity could not be continued. If you do not implement this method, UIKit displays an error to the user with an appropriate message about the reason for the failure.

This method is not called if either application(_:willFinishLaunchingWithOptions:) or application(_:didFinishLaunchingWithOptions:) returns false.

## See Also

### Continuing user activity and handling quick actions

func application(UIApplication, willContinueUserActivityWithType: String) -> Bool

Tells the delegate if your app takes responsibility for notifying users when a continuation activity takes longer than expected.

func application(UIApplication, continue: NSUserActivity, restorationHandler: ([any UIUserActivityRestoring]?) -> Void) -> Bool

Tells the delegate that the data for continuing an activity is available.

func application(UIApplication, didUpdate: NSUserActivity)

Tells the delegate that the activity was updated.

func application(UIApplication, performActionFor: UIApplicationShortcutItem, completionHandler: (Bool) -> Void)

Tells the delegate that the user selected a Home screen quick action for your app, except when you’ve intercepted the interaction in a launch method.

