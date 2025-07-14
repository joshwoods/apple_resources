

- User Notifications
- UNNotificationActionOptions
-  authenticationRequired 

Type Property

# authenticationRequired

The action can be performed only on an unlocked device.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.14+visionOS 1.0+watchOS 3.0+

``` source
static var authenticationRequired: UNNotificationActionOptions { get }
```

## Discussion

When the user selects an action with this option, the system prompts the user to unlock the device. After unlocking, the system notifies your app of the selected action. You might use option to perform actions that require accessing data that is encrypted while the device is locked.

## See Also

### Constants

static var destructive: UNNotificationActionOptions

The action performs a destructive task.

static var foreground: UNNotificationActionOptions

The action causes the app to launch in the foreground.

