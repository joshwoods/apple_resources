

- WatchKit
-  WKRefreshBackgroundTask 

Class

# WKRefreshBackgroundTask

The abstract superclass for WatchKit’s background task classes.

watchOS 3.0+

``` source
class WKRefreshBackgroundTask
```

## Mentioned in 

Preparing to take your watchOS app’s snapshot

Using background tasks

## Overview

Don’t subclass or create instances of this class. The system automatically creates an appropriate background task object whenever it triggers a background task. This object is passed to your app delegate’s handle(_:) method. Use the provided background task object to identify and manage the background task.

Note

In watchOS 9 and later, SwiftUI Background tasks are the preferred way to handle background tasks and interactions. For more information, see backgroundTask(_:action:).

## Topics

### Accessing background task data

var userInfo: (any NSSecureCoding &amp; NSObjectProtocol)?

Custom information associated with the background task.

### Completing the background task

var expirationHandler: (() -> Void)?

A block that the system calls when the available runtime for a background task is about to expire.

func setTaskCompletedWithSnapshot(Bool)

Marks the task as complete and indicates whether the system should take a new snapshot of the app.

func setTaskCompleted()

Marks the task as complete.

Deprecated

## Relationships

### Inherits From

- NSObject

### Inherited By

- WKApplicationRefreshBackgroundTask
- WKBluetoothAlertRefreshBackgroundTask
- WKIntentDidRunRefreshBackgroundTask
- WKRelevantShortcutRefreshBackgroundTask
- WKSnapshotRefreshBackgroundTask
- WKURLSessionRefreshBackgroundTask
- WKWatchConnectivityRefreshBackgroundTask

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

class WKApplicationRefreshBackgroundTask

A task that updates your app’s state in the background.

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

