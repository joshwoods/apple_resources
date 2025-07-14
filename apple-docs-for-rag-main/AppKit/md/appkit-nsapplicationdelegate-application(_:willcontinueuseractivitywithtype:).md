

- AppKit
- NSApplicationDelegate
-  application(\_:willContinueUserActivityWithType:) 

Instance Method

# application(\_:willContinueUserActivityWithType:)

Returns a Boolean value that indicates if the app can continue the specified activity.

macOS 10.10+

``` source
@MainActor
optional func application(
    _ application: NSApplication,
    willContinueUserActivityWithType userActivityType: String
) -> Bool
```

## Parameters 

`application`  

The app continuing the user activity.

`userActivityType`  

The type of activity to be continued.

## Return Value

true if you notify the user that your app is about to continue the activity or false if you want AppKit to notify the user.

## Discussion

Use this method to provide immediate feedback to the user that an activity is about to continue on this device. The app calls this method as soon as the user confirms that an activity should be continued but possibly before the data associated with that activity is available.

This method is called on the main thread as soon as the user indicates they want to continue an activity in your app. The `NSUserActivity` object may not be available instantly, so use this as an opportunity to show the user that an activity will be continued shortly and return true. If you leave this method unimplemented or return false, AppKit displays a default indication.

For each invocation of this method, the app delegate is guaranteed to get exactly one invocation of application(_:continue:restorationHandler:) on success, or application(_:didFailToContinueUserActivityWithType:error:) if an error was encountered.

## See Also

### Continuing User Activities

func application(NSApplication, continue: NSUserActivity, restorationHandler: ([any NSUserActivityRestoring]) -> Void) -> Bool

Returns a Boolean value that indicates if the app successfully recreates the specified activity.

func application(NSApplication, didFailToContinueUserActivityWithType: String, error: any Error)

Tells the delegate that the app couldn’t continue the specified activity.

func application(NSApplication, didUpdate: NSUserActivity)

Tells the delegate that there are changes to the specified activity.

