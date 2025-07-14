

- WatchKit
- WKUserNotificationInterfaceController
-  performNotificationDefaultAction() 

Instance Method

# performNotificationDefaultAction()

Launches the watchOS app and performs the current notification’s default action.

watchOS 5.0+

``` source
@MainActor
func performNotificationDefaultAction()
```

## See Also

### Working with Actions

var notificationActions: [UNNotificationAction]

The actions associated with the current notification.

func performDismissAction()

Dismisses the notification interface controller.

func dismiss()

Dismisses the notification interface controller.

Deprecated

