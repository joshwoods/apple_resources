

- WatchKit
-  WKIntentDidRunRefreshBackgroundTask 

Class

# WKIntentDidRunRefreshBackgroundTask

A background task used to update your app after a SiriKit intent runs.

watchOS 5.0+

``` source
class WKIntentDidRunRefreshBackgroundTask
```

## Mentioned in 

Using background tasks

## Overview

Intent-based shortcuts can update your app’s state; however, the intent executes in a separate process from your WatchKit extension. To update the app, the system schedules this task whenever one of your intents finishes executing. Use this task to check for any updates to your app’s state, and to make sure its visible interfaces are current. For example, you can update all of your app’s snapshot, complications, and relevant shortcuts.

Don’t subclass or create instances of this class. Instead, the system instantiates a WKIntentDidRunRefreshBackgroundTask object and passes the task object to your app delegate’s handle(_:) method.

Note

In watchOS 9 and later, SwiftUI Background tasks are the preferred way to handle background tasks and interactions. For more information, backgroundTask(_:action:).

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

class WKApplicationRefreshBackgroundTask

A task that updates your app’s state in the background.

class WKURLSessionRefreshBackgroundTask

A task that responds to background URL sessions.

class WKWatchConnectivityRefreshBackgroundTask

A background task used to receive background updates from the Watch Connectivity framework.

class WKBluetoothAlertRefreshBackgroundTask

A task for handling timely Bluetooth alerts in the background.

class WKRelevantShortcutRefreshBackgroundTask

A background task used to periodically donate relevant Siri shortcuts.

class WKSnapshotRefreshBackgroundTask

A background task used to update your app’s user interface in preparation for a snapshot.

class WKRefreshBackgroundTask

The abstract superclass for WatchKit’s background task classes.

