

- User Notifications
-  UNNotificationPresentationOptionNone 

Global Variable

# UNNotificationPresentationOptionNone

No alert.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.14+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
static const UNNotificationPresentationOptions UNNotificationPresentationOptionNone;
```

## Discussion

Specify this constant when you want to silence any user interactions for a notification.

## See Also

### Receiving Notifications

func userNotificationCenter(UNUserNotificationCenter, willPresent: UNNotification, withCompletionHandler: (UNNotificationPresentationOptions) -> Void)

Asks the delegate how to handle a notification that arrived while the app was running in the foreground.

struct UNNotificationPresentationOptions

Constants indicating how to present a notification in a foreground app.

