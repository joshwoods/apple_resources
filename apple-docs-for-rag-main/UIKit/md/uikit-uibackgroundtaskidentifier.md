

- UIKit
-  UIBackgroundTaskIdentifier 

Structure

# UIBackgroundTaskIdentifier

A unique token that identifies a request to run in the background.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
struct UIBackgroundTaskIdentifier
```

## Topics

### Identifier

static let invalid: UIBackgroundTaskIdentifier

A token that indicates an invalid task request.

### Initializers

init(rawValue: Int)

Creates a new instance with the specified raw value.

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

enum UIBackgroundRefreshStatus

Constants that indicate whether background execution is enabled for the app.

class let backgroundRefreshStatusDidChangeNotification: NSNotification.Name

A notification that posts when the app’s status for downloading content in the background changes.

func beginBackgroundTask(withName: String?, expirationHandler: (() -> Void)?) -> UIBackgroundTaskIdentifier

Marks the start of a task with a custom name that should continue if the app enters the background.

func beginBackgroundTask(expirationHandler: (() -> Void)?) -> UIBackgroundTaskIdentifier

Marks the start of a task that should continue if the app enters the background.

func endBackgroundTask(UIBackgroundTaskIdentifier)

Marks the end of a specific long-running background task.

var backgroundTimeRemaining: TimeInterval

The maximum amount of time remaining for the app to run in the background.

