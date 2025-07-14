

- User Notifications
- UNUserNotificationCenter
-  supportsContentExtensions 

Instance Property

# supportsContentExtensions

A Boolean value that indicates whether the device supports notification content extensions.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.14+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
var supportsContentExtensions: Bool { get }
```

## Discussion

Notification content extensions let you customize the appearance of the alerts displayed for your app’s notifications. The value of this property is true for devices that support notification content extensions and false for devices that do not support them. For information about how to implement a notification content extension, see Customizing the Appearance of Notifications.

## See Also

### Processing received notifications

var delegate: (any UNUserNotificationCenterDelegate)?

The notification center’s delegate.

protocol UNUserNotificationCenterDelegate

An interface for processing incoming notifications and responding to notification actions.

