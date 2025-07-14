

- WatchKit
-  WKBluetoothAlertRefreshBackgroundTask 

Class

# WKBluetoothAlertRefreshBackgroundTask

A task for handling timely Bluetooth alerts in the background.

watchOS 9.0+

``` source
class WKBluetoothAlertRefreshBackgroundTask
```

## Mentioned in 

Using background tasks

## Overview

Your app can receive WKBluetoothAlertRefreshBackgroundTask tasks to handle timely alerts in the background. Use these tasks to reconnect a peripheral and handle a critical alert. Apps that use timely alerts can also scan for a specific system identifier (UUID) while in the background. You can then perform the initial connection and pair the devices if necessary.

To receive timely alerts, your peripheral must use Generic Attribute Profile (GATT) transactions. Call setNotifyValue(_:for:) to enable notifications for the specified characteristic. Then, any changes to the peripheral’s characteristic wakes your app using a WKBluetoothAlertRefreshBackgroundTask task. Use this task to reconnect to the peripheral and handle the critical alert.

Note

In watchOS 9 and later, SwiftUI Background tasks are the preferred way to handle background tasks and interactions. For more information, backgroundTask(_:action:).

The critical alerts and background scans share a budget. Your app can only use five timely alerts or background scans within a rolling 24-hour window.

When your app receives a timely alert and your budget has only one Bluetooth alert task remaining, the system raises a leGattNearBackgroundNotificationLimit error. If you exceed the budget, it raises a leGattExceededBackgroundNotificationLimit error. The system passes these errors to your CBPeripheralDelegate, by calling methods like the peripheral(_:didUpdateValueFor:error:) method.

If you exceed your budget, your app doesn’t receive any timely alerts until additional background budget becomes available. The user can reset this budget by launching your app.

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

class WKIntentDidRunRefreshBackgroundTask

A background task used to update your app after a SiriKit intent runs.

class WKRelevantShortcutRefreshBackgroundTask

A background task used to periodically donate relevant Siri shortcuts.

class WKSnapshotRefreshBackgroundTask

A background task used to update your app’s user interface in preparation for a snapshot.

class WKRefreshBackgroundTask

The abstract superclass for WatchKit’s background task classes.

