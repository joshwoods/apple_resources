

- WatchKit
- WKUserNotificationInterfaceController
-  notificationActions 

Instance Property

# notificationActions

The actions associated with the current notification.

watchOS 5.0+

``` source
@MainActor
var notificationActions: [UNNotificationAction] { get set }
```

## Discussion

Use this array to dynamically update the list of actions associated with a notification. You can only change this property during the didReceive(_:) method.

## See Also

### Related Documentation

func didReceive(UNNotification)

Delivers a notification object to your interface controller for processing.

### Working with Actions

func performNotificationDefaultAction()

Launches the watchOS app and performs the current notification’s default action.

func performDismissAction()

Dismisses the notification interface controller.

func dismiss()

Dismisses the notification interface controller.

Deprecated

