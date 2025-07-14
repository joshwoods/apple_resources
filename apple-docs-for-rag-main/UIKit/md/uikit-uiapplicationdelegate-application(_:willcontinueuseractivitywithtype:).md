

- UIKit
- UIApplicationDelegate
-  application(\_:willContinueUserActivityWithType:) 

Instance Method

# application(\_:willContinueUserActivityWithType:)

Tells the delegate if your app takes responsibility for notifying users when a continuation activity takes longer than expected.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
optional func application(
    _ application: UIApplication,
    willContinueUserActivityWithType userActivityType: String
) -> Bool
```

## Parameters 

`application`  

Your shared app object.

`userActivityType`  

The requested activity type.

## Return Value

true if you want to notify the user that a continuation is in progress or false if you want iOS to notify the user.

## Discussion

Use this method to provide immediate feedback to the user that an activity is about to continue on this device. The app calls this method as soon as the user confirms that an activity should be continued but possibly before the data associated with that activity is available.

Your implementation of this method should prepare to initiate the activity. If you notify the user as part of your preparations, return true from this method so that iOS does not also notify the user. If you do not implement this method or your implementation returns false, iOS notifes the user.

This method is not called if either application(_:willFinishLaunchingWithOptions:) or application(_:didFinishLaunchingWithOptions:) returns false.

## See Also

### Continuing user activity and handling quick actions

func application(UIApplication, continue: NSUserActivity, restorationHandler: ([any UIUserActivityRestoring]?) -> Void) -> Bool

Tells the delegate that the data for continuing an activity is available.

func application(UIApplication, didUpdate: NSUserActivity)

Tells the delegate that the activity was updated.

func application(UIApplication, didFailToContinueUserActivityWithType: String, error: any Error)

Tells the delegate that the activity couldn’t be continued.

func application(UIApplication, performActionFor: UIApplicationShortcutItem, completionHandler: (Bool) -> Void)

Tells the delegate that the user selected a Home screen quick action for your app, except when you’ve intercepted the interaction in a launch method.

