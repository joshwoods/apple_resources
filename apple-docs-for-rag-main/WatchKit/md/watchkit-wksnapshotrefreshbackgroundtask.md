

- WatchKit
-  WKSnapshotRefreshBackgroundTask 

Class

# WKSnapshotRefreshBackgroundTask

A background task used to update your app’s user interface in preparation for a snapshot.

watchOS 3.0+

``` source
class WKSnapshotRefreshBackgroundTask
```

## Mentioned in 

Preparing to take your watchOS app’s snapshot

## Overview

Using the methods of WKSnapshotRefreshBackgroundTask, you can push, pop, or present other interface controllers, and then update the content of the desired interface controller. The system automatically takes a snapshot of your user interface as soon as this task completes.

Don’t subclass or create instances of this class. Instead, schedule a background snapshot refresh task by calling scheduleSnapshotRefresh(withPreferredDate:userInfo:scheduledCompletion:). When the system triggers this task, it launches your app in the background, instantiates a WKSnapshotRefreshBackgroundTask object, and passes the task object to your app delegate’s handle(_:) method.

Note

In watchOS 9 and later, SwiftUI Background tasks are the preferred way to handle background tasks and interactions. For more information, backgroundTask(_:action:).

Background snapshot tasks are budgeted. In general, the system performs approximately one task per hour for each app in the dock (including the most recently used app). This budget is shared among all apps on the dock. The system performs multiple tasks an hour for each app with a complication on the active watch face. This budget is shared among all complications on the watch face. After you exhaust the budget, the system delays your requests until more time becomes available.

The system automatically schedules background snapshot request tasks when:

- Your device starts up

- Your app updates the complication timeline

- The user interacts with one of the apps notifications

- The app transitions from the foreground to the background

- One hour passes after the user’s last interaction with the app, then the `returnToGlanceableUI` property is set to true

These requests don’t cancel or replace any of your scheduled requests.

## Topics

### Completing the background task

func setTaskCompleted(restoredDefaultState: Bool, estimatedSnapshotExpiration: Date?, userInfo: (any NSSecureCoding &amp; NSObjectProtocol)?)

Marks the task as complete.

### Instance properties

var reasonForSnapshot: WKSnapshotReason

The reason for taking the upcoming snapshot.

enum WKSnapshotReason

The reason for a background snapshot task.

var returnToDefaultState: Bool

A Boolean value indicating that the app should return to its default state.

Deprecated

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

class WKIntentDidRunRefreshBackgroundTask

A background task used to update your app after a SiriKit intent runs.

class WKRelevantShortcutRefreshBackgroundTask

A background task used to periodically donate relevant Siri shortcuts.

class WKRefreshBackgroundTask

The abstract superclass for WatchKit’s background task classes.

