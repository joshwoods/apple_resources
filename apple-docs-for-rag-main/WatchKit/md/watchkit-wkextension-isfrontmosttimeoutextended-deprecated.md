

- WatchKit
- WKExtension
-  isFrontmostTimeoutExtended Deprecated

Instance Property

# isFrontmostTimeoutExtended

A Boolean value that determines whether the app extends its time as the frontmost app.

watchOS 4.0–7.0Deprecated

``` source
@MainActor
var isFrontmostTimeoutExtended: Bool { get set }
```

Deprecated

In watchOS 7 and later, you can no longer request extended frontmost time. Instead, the user can set the frontmost app behavior for each app using its Return to App setting.

## Mentioned in 

Taking Advantage of Frontmost App State

## Discussion

This value defaults to false. An app remains the frontmost app for two minutes after the user drops their wrist. Setting this property to true extends the app’s time as the frontmost app to eight minutes.

Don’t just extend the app’s frontmost time globally. Instead, enable it only when the user performs an activity that they are likely to continue. Otherwise, disable it. Users can also change the default length of time that apps spend as the frontmost app by choosing Settings \> General \> Wake Screen. If they select a time that is eight minutes or longer, this property has no effect. In other words, when isFrontmostTimeoutExtended is true, the app remains the frontmost app for eight minutes, or for the amount of time that the user selects, whichever is longer.

## See Also

### Managing the execution state

var applicationState: WKApplicationState

The runtime state of the Watch app.

enum WKApplicationState

The running states of the Watch app.

var isApplicationRunningInDock: Bool

A Boolean value that indicates whether the app is running in the dock.

func scheduleBackgroundRefresh(withPreferredDate: Date, userInfo: (any NSSecureCoding &amp; NSObjectProtocol)?, scheduledCompletion: ((any Error)?) -> Void)

Schedules a background task to refresh the app’s data.

