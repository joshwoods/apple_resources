

- UIKit
- UIApplication
-  endBackgroundTask(\_:) 

Instance Method

# endBackgroundTask(\_:)

Marks the end of a specific long-running background task.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
nonisolated
func endBackgroundTask(_ identifier: UIBackgroundTaskIdentifier)
```

## Parameters 

`identifier`  

An identifier returned by the beginBackgroundTask(expirationHandler:) method.

## Mentioned in 

Extending your app’s background execution time

## Discussion

You must call this method to end a task that was started using the beginBackgroundTask(expirationHandler:) method. If you do not, the system may terminate your app.

This method can be safely called on a non-main thread.

## See Also

### Managing background tasks

var backgroundRefreshStatus: UIBackgroundRefreshStatus

Indicates whether the app can refresh content when running in the background.

enum UIBackgroundRefreshStatus

Constants that indicate whether background execution is enabled for the app.

class let backgroundRefreshStatusDidChangeNotification: NSNotification.Name

A notification that posts when the app’s status for downloading content in the background changes.

func beginBackgroundTask(withName: String?, expirationHandler: (() -> Void)?) -> UIBackgroundTaskIdentifier

Marks the start of a task with a custom name that should continue if the app enters the background.

func beginBackgroundTask(expirationHandler: (() -> Void)?) -> UIBackgroundTaskIdentifier

Marks the start of a task that should continue if the app enters the background.

struct UIBackgroundTaskIdentifier

A unique token that identifies a request to run in the background.

var backgroundTimeRemaining: TimeInterval

The maximum amount of time remaining for the app to run in the background.

