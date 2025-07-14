

- UIKit
-  UIBackgroundRefreshStatus 

Enumeration

# UIBackgroundRefreshStatus

Constants that indicate whether background execution is enabled for the app.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOS 11.0+visionOS 1.0+

``` source
enum UIBackgroundRefreshStatus
```

## Topics

### Constants

case restricted

Background updates are unavailable and the user cannot enable them again.

case denied

The user explicitly disabled background behavior for this app or for the whole system.

case available

Background updates are available for the app.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Managing background tasks

var backgroundRefreshStatus: UIBackgroundRefreshStatus

Indicates whether the app can refresh content when running in the background.

class let backgroundRefreshStatusDidChangeNotification: NSNotification.Name

A notification that posts when the app’s status for downloading content in the background changes.

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

