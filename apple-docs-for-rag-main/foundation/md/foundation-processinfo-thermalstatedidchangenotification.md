

- Foundation
- ProcessInfo
-  thermalStateDidChangeNotification 

Type Property

# thermalStateDidChangeNotification

Posts when the thermal state of the system changes.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.10.3+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
class let thermalStateDidChangeNotification: NSNotification.Name
```

## Discussion

The notification object is a ProcessInfo instance.

To receive thermalStateDidChangeNotification, you must access the thermalState prior to registering for the notification.

## See Also

### Notifications

static let NSProcessInfoPowerStateDidChange: NSNotification.Name

Posts when the power state of a device changes.

