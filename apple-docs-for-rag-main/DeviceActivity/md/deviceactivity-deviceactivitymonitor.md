

- DeviceActivity
-  DeviceActivityMonitor 

Class

# DeviceActivityMonitor

The object that monitors scheduled device activity.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+

``` source
@objc
class DeviceActivityMonitor
```

## Overview

`DeviceActivityMonitor` provides the entry point into a device activity monitor extension. You should subclass `DeviceActivityMonitor` and designate your subclass as the principal class of your app extension.

The following code implements `DeviceActivityMonitor` in an app:

```
class MyMonitorExtension: DeviceActivityMonitor {
  let store = ManagedSettingsStore()

  // You can use the `store` property to shield apps when an interval starts, ends, or meets a threshold.
  override func intervalDidStart(for activity: DeviceActivityName) {
      super.intervalDidStart(for: activity)

      // Shield selected applications.
      let model = MyModel()
      let applications = model.selectionToShield.applications
      store.shield.applications = applications.isEmpty ? nil : applications
   }
```

Note

Shielding an app dims the app’s icon on the homescreen and applies an hourglass symbol. When the app launches, the system covers it with a view that your app can configure.

## Topics

### Configuring a Monitor

init()

Creates a new monitor implemented by subclasses.

### Monitoring Scheduled Intervals

func intervalDidEnd(for: DeviceActivityName)

Indicates that the device activity interval ended.

func intervalDidStart(for: DeviceActivityName)

Indicates that the device activity interval started.

func intervalWillEndWarning(for: DeviceActivityName)

Warns your app of an ongoing activity’s conclusion a specified time before the activity ends.

func intervalWillStartWarning(for: DeviceActivityName)

Warns your app of an upcoming activity a specified time before the activity starts.

### Monitoring Event Thresholds

func eventDidReachThreshold(DeviceActivityEvent.Name, activity: DeviceActivityName)

Indicates that the activity reached its threshold.

func eventWillReachThresholdWarning(DeviceActivityEvent.Name, activity: DeviceActivityName)

Warns your app that an activity is about to reach its threshold.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

