

- WatchKit
- WKExtension
-  applicationState 

Instance Property

# applicationState

The runtime state of the Watch app.

watchOS 3.0+

``` source
@MainActor
var applicationState: WKApplicationState { get }
```

## Discussion

The Watch app may be active, inactive, or running in the background. Use this property to get the current state. To be notified of state changes, implement the appropriate methods of the delegate object.

## See Also

### Managing the execution state

enum WKApplicationState

The running states of the Watch app.

var isApplicationRunningInDock: Bool

A Boolean value that indicates whether the app is running in the dock.

func scheduleBackgroundRefresh(withPreferredDate: Date, userInfo: (any NSSecureCoding &amp; NSObjectProtocol)?, scheduledCompletion: ((any Error)?) -> Void)

Schedules a background task to refresh the app’s data.

var isFrontmostTimeoutExtended: Bool

A Boolean value that determines whether the app extends its time as the frontmost app.

Deprecated

