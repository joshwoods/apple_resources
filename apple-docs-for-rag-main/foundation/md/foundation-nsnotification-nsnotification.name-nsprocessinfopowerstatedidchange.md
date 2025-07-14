

- Foundation
- NSNotification
- NSNotification.Name
-  NSProcessInfoPowerStateDidChange 

Type Property

# NSProcessInfoPowerStateDidChange

Posts when the power state of a device changes.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 12.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static let NSProcessInfoPowerStateDidChange: NSNotification.Name
```

## Discussion

After your observer receives this notification, query the isLowPowerModeEnabled property to determine the current power state of the device. If Low Power Mode is active, take appropriate steps to reduce activity in your app. Otherwise, your app can resume normal operations.

The notification object is a ProcessInfo instance.

## See Also

### Related Documentation

func addObserver(Any, selector: Selector, name: NSNotification.Name?, object: Any?)

Adds an entry to the notification center to call the provided selector with the notification.

var isLowPowerModeEnabled: Bool

A Boolean value that indicates the current state of Low Power Mode.

class NotificationCenter

A notification dispatch mechanism that enables the broadcast of information to registered observers.

### Notifications

class let thermalStateDidChangeNotification: NSNotification.Name

Posts when the thermal state of the system changes.

