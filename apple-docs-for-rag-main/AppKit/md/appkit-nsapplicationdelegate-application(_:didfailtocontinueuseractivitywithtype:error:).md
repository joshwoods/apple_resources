

- AppKit
- NSApplicationDelegate
-  application(\_:didFailToContinueUserActivityWithType:error:) 

Instance Method

# application(\_:didFailToContinueUserActivityWithType:error:)

Tells the delegate that the app couldn’t continue the specified activity.

macOS 10.10+

``` source
@MainActor
optional func application(
    _ application: NSApplication,
    didFailToContinueUserActivityWithType userActivityType: String,
    error: any Error
)
```

## Parameters 

`application`  

The app that attempted to continue the activity.

`userActivityType`  

The activity type that was attempted.

`error`  

An error object indicating the reason for the failure.

## Discussion

Use this method to let the user know that the specified activity could not be continued. If you do not implement this method, AppKit displays an error to the user with an appropriate message about the reason for the failure.

## See Also

### Continuing User Activities

func application(NSApplication, willContinueUserActivityWithType: String) -> Bool

Returns a Boolean value that indicates if the app can continue the specified activity.

func application(NSApplication, continue: NSUserActivity, restorationHandler: ([any NSUserActivityRestoring]) -> Void) -> Bool

Returns a Boolean value that indicates if the app successfully recreates the specified activity.

func application(NSApplication, didUpdate: NSUserActivity)

Tells the delegate that there are changes to the specified activity.

