

- WatchKit
- WKApplication
-  applicationState 

Instance Property

# applicationState

The runtime state of the watchOS app.

watchOS 7.0+

``` source
@MainActor
var applicationState: WKApplicationState { get }
```

## Discussion

The watchOS app may be active, inactive, or running in the background. Use this property to get the current state. To receive notifications about state changes, implement the appropriate methods of the WKApplicationDelegate object, or create a SwiftUI view that updates based on changes to the ScenePhase environment value.

## See Also

### Managing the app state

enum WKApplicationState

The running states of the Watch app.

var isApplicationRunningInDock: Bool

A Boolean value that indicates whether the app is running in the dock.

func scheduleBackgroundRefresh(withPreferredDate: Date, userInfo: (any NSSecureCoding &amp; NSObjectProtocol)?, scheduledCompletion: ((any Error)?) -> Void)

Schedules a background task to refresh the app’s data.

