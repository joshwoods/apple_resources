

- Foundation
- ProcessInfo
-  isLowPowerModeEnabled 

Instance Property

# isLowPowerModeEnabled

A Boolean value that indicates the current state of Low Power Mode.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 12.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var isLowPowerModeEnabled: Bool { get }
```

## Discussion

Users who wish to prolong their device’s battery life can enable Low Power Mode under Settings \> Battery. In Low Power Mode, the system conserves battery life by enacting certain energy-saving measures, such as:

- Reducing CPU and GPU performance.

- Reducing screen brightness.

- Pausing discretionary and background activities.

Your app can query the isLowPowerModeEnabled property at any time to determine whether Low Power Mode is active.

Your app can also register to receive notifications when the Low Power Mode state of a device changes. To register for power state notifications, send the message addObserver(_:selector:name:object:) to the default notification center of your app (an instance of NotificationCenter). Pass it a selector to call and a notification name of NSProcessInfoPowerStateDidChange. When your app receives a notification of a power state change, query isLowPowerModeEnabled to determine the current power state. If Low Power Mode is active, take appropriate steps to reduce activity in your app. Otherwise, your app can resume normal operations.

For additional information, see React to Low Power Mode on iPhones in Energy Efficiency Guide for iOS Apps.

## See Also

### Related Documentation

static let NSProcessInfoPowerStateDidChange: NSNotification.Name

Posts when the power state of a device changes.

func addObserver(Any, selector: Selector, name: NSNotification.Name?, object: Any?)

Adds an entry to the notification center to call the provided selector with the notification.

class NotificationCenter

A notification dispatch mechanism that enables the broadcast of information to registered observers.

