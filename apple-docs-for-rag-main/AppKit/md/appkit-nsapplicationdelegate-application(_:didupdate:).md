

- AppKit
- NSApplicationDelegate
-  application(\_:didUpdate:) 

Instance Method

# application(\_:didUpdate:)

Tells the delegate that there are changes to the specified activity.

macOS 10.10+

``` source
@MainActor
optional func application(
    _ application: NSApplication,
    didUpdate userActivity: NSUserActivity
)
```

## Parameters 

`application`  

The shared app object.

`userActivity`  

The user activity object that was updated.

## Discussion

This method is called when any user activity managed by AppKit has been updated. Use this as a last chance to add additional data to the user activity object.

## See Also

### Continuing User Activities

func application(NSApplication, willContinueUserActivityWithType: String) -> Bool

Returns a Boolean value that indicates if the app can continue the specified activity.

func application(NSApplication, continue: NSUserActivity, restorationHandler: ([any NSUserActivityRestoring]) -> Void) -> Bool

Returns a Boolean value that indicates if the app successfully recreates the specified activity.

func application(NSApplication, didFailToContinueUserActivityWithType: String, error: any Error)

Tells the delegate that the app couldn’t continue the specified activity.

