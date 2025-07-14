

- User Notifications
- UNNotificationActionOptions
-  foreground 

Type Property

# foreground

The action causes the app to launch in the foreground.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.14+visionOS 1.0+watchOS 3.0+

``` source
static var foreground: UNNotificationActionOptions { get }
```

## Discussion

When the user selects an action containing this option, the system brings the app to the foreground, asking the user to unlock the device as needed. Use this option for actions that require the user to interact further with your app. Do not use this option simply to bring your app to the foreground.

## See Also

### Constants

static var authenticationRequired: UNNotificationActionOptions

The action can be performed only on an unlocked device.

static var destructive: UNNotificationActionOptions

The action performs a destructive task.

