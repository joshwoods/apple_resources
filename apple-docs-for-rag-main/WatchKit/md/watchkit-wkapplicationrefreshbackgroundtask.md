

- WatchKit
-  WKApplicationRefreshBackgroundTask 

Class

# WKApplicationRefreshBackgroundTask

A task that updates your app’s state in the background.

watchOS 3.0+

``` source
class WKApplicationRefreshBackgroundTask
```

## Mentioned in 

Using background tasks

## Overview

Don’t subclass or create instances of this class. Instead, schedule a background app refresh task by calling scheduleBackgroundRefresh(withPreferredDate:userInfo:scheduledCompletion:). When the system triggers the background task, it launches your app in the background, instantiates a WKApplicationRefreshBackgroundTask object, and passes the task object to your app delegate’s handle(_:) method.

Note

In watchOS 9 and later, SwiftUI Background tasks are the preferred way to handle background tasks and interactions. For more information, backgroundTask(_:action:).

The system budgets the number of background refresh tasks available to an app. In general, the system performs approximately four tasks per hour for each app with a complication on the active watch face. All the complications on the current watch face share this budget. After you exhaust the budget, the system delays your requests until more time becomes available.

## Relationships

### Inherits From

- WKRefreshBackgroundTask

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

## See Also

### Background tasks

Using background tasks

Handle scheduled update tasks in the background, and respond to background system interactions including Siri intents and incoming Bluetooth messages.

Preparing to take your watchOS app’s snapshot

Provide a timely, accurate snapshot of your app by using snapshot background tasks.

class WKURLSessionRefreshBackgroundTask

A task that responds to background URL sessions.

class WKWatchConnectivityRefreshBackgroundTask

A background task used to receive background updates from the Watch Connectivity framework.

class WKBluetoothAlertRefreshBackgroundTask

A task for handling timely Bluetooth alerts in the background.

class WKIntentDidRunRefreshBackgroundTask

A background task used to update your app after a SiriKit intent runs.

class WKRelevantShortcutRefreshBackgroundTask

A background task used to periodically donate relevant Siri shortcuts.

class WKSnapshotRefreshBackgroundTask

A background task used to update your app’s user interface in preparation for a snapshot.

class WKRefreshBackgroundTask

The abstract superclass for WatchKit’s background task classes.

