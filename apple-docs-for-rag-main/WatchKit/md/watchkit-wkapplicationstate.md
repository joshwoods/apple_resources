

- WatchKit
-  WKApplicationState 

Enumeration

# WKApplicationState

The running states of the Watch app.

watchOS 3.0+

``` source
enum WKApplicationState
```

## Topics

### Constants

case active

The Watch app is running in the foreground and currently receiving events.

case inactive

The Watch app is running in the foreground, but is not yet responding to actions from controls or gestures.

case background

The Watch app is running in the background.

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

### Managing the app state

var applicationState: WKApplicationState

The runtime state of the watchOS app.

var isApplicationRunningInDock: Bool

A Boolean value that indicates whether the app is running in the dock.

func scheduleBackgroundRefresh(withPreferredDate: Date, userInfo: (any NSSecureCoding &amp; NSObjectProtocol)?, scheduledCompletion: ((any Error)?) -> Void)

Schedules a background task to refresh the app’s data.

