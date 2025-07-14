

- WatchKit
- WKApplication
-  isApplicationRunningInDock 

Instance Property

# isApplicationRunningInDock

A Boolean value that indicates whether the app is running in the dock.

watchOS 7.0+

``` source
@MainActor
var isApplicationRunningInDock: Bool { get }
```

## Discussion

This property contains true if the app is running in the dock; otherwise, false.

Check this property (for example, in your app delegate’s applicationWillEnterForeground() method) to determine whether your app is running in the dock. You can use this information to customize your user interface in the dock.

## See Also

### Managing the app state

var applicationState: WKApplicationState

The runtime state of the watchOS app.

enum WKApplicationState

The running states of the Watch app.

func scheduleBackgroundRefresh(withPreferredDate: Date, userInfo: (any NSSecureCoding &amp; NSObjectProtocol)?, scheduledCompletion: ((any Error)?) -> Void)

Schedules a background task to refresh the app’s data.

