

- WatchKit
- WKUserNotificationInterfaceController
-  dismiss() Deprecated

Instance Method

# dismiss()

Dismisses the notification interface controller.

watchOS 2.0–5.0Deprecated

``` source
@MainActor
func dismiss()
```

Deprecated

Use performDismissAction() instead.

## See Also

### Working with Actions

var notificationActions: [UNNotificationAction]

The actions associated with the current notification.

func performNotificationDefaultAction()

Launches the watchOS app and performs the current notification’s default action.

func performDismissAction()

Dismisses the notification interface controller.

