

- User Notifications
- UNNotificationActionOptions
-  destructive 

Type Property

# destructive

The action performs a destructive task.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.14+visionOS 1.0+watchOS 3.0+

``` source
static var destructive: UNNotificationActionOptions { get }
```

## Mentioned in 

Declaring your actionable notification types

## Discussion

Use this option for actions that delete user data or change the app irrevocably. The action button is displayed with special highlighting to indicate that it performs a destructive task.

## See Also

### Constants

static var authenticationRequired: UNNotificationActionOptions

The action can be performed only on an unlocked device.

static var foreground: UNNotificationActionOptions

The action causes the app to launch in the foreground.

