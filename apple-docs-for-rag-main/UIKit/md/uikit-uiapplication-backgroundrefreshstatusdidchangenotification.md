

- UIKit
- UIApplication
-  backgroundRefreshStatusDidChangeNotification 

Type Property

# backgroundRefreshStatusDidChangeNotification

A notification that posts when the app’s status for downloading content in the background changes.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOS 11.0+visionOS 1.0+

``` source
nonisolated
class let backgroundRefreshStatusDidChangeNotification: NSNotification.Name
```

## Discussion

The system sends this notification when the backgroundRefreshStatus property of the app object changes. That property can change in response to the user disabling multitasking support for the app. The `object` of the notification is the `UIApplication` object. There is no `userInfo` dictionary.

## See Also

### Managing background tasks

var backgroundRefreshStatus: UIBackgroundRefreshStatus

Indicates whether the app can refresh content when running in the background.

enum UIBackgroundRefreshStatus

Constants that indicate whether background execution is enabled for the app.

func beginBackgroundTask(withName: String?, expirationHandler: (() -> Void)?) -> UIBackgroundTaskIdentifier

Marks the start of a task with a custom name that should continue if the app enters the background.

func beginBackgroundTask(expirationHandler: (() -> Void)?) -> UIBackgroundTaskIdentifier

Marks the start of a task that should continue if the app enters the background.

func endBackgroundTask(UIBackgroundTaskIdentifier)

Marks the end of a specific long-running background task.

struct UIBackgroundTaskIdentifier

A unique token that identifies a request to run in the background.

var backgroundTimeRemaining: TimeInterval

The maximum amount of time remaining for the app to run in the background.

