

- AppKit
- NSWorkspace
-  notificationCenter 

Instance Property

# notificationCenter

The notification center for workspace notifications.

macOS

``` source
var notificationCenter: NotificationCenter { get }
```

## Return Value

The notification center object associated with the workspace

## Discussion

This notification center object delivers the workspace-related notifications described in Responding to Environment Notifications.

You can access this object safely from any thread in your app in macOS 10.6 and later.

