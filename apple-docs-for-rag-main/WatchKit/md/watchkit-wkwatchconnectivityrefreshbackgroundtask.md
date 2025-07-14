

- WatchKit
-  WKWatchConnectivityRefreshBackgroundTask 

Class

# WKWatchConnectivityRefreshBackgroundTask

A background task used to receive background updates from the Watch Connectivity framework.

watchOS 3.0+

``` source
class WKWatchConnectivityRefreshBackgroundTask
```

## Mentioned in 

Using background tasks

## Overview

Don’t subclass or create instances of this class. Instead, when this background watch connectivity task is triggered, the system launches your app in the background, instantiates a WKWatchConnectivityRefreshBackgroundTask object, and passes the task object to your app delegate’s handle(_:) method.

Note

In watchOS 9 and later, SwiftUI Background tasks are the preferred way to handle background tasks and interactions. For more information, backgroundTask(_:action:).

Background watch connectivity tasks are triggered whenever the paired device sends data using one of the following WCSession methods:

- updateApplicationContext(_:)

- transferUserInfo(_:)

- transferCurrentComplicationUserInfo(_:)

- transferFile(_:metadata:)

The background watch connectivity task informs you that your app is given background time. You must use your WCSessionDelegate methods to receive this data. Because of the asynchronous nature of these tasks, defer calling your tasks’s setTaskCompleted() method until after you’ve activated your session and received all the pending data. Use the hasContentPending property to determine whether you still have any pending data.

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

