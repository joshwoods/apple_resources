

- CloudKit
- CKSubscription
- CKSubscription.NotificationInfo
-  category 

Instance Property

# category

The name of the action group that corresponds to this notification.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+watchOS 2.0+

``` source
var category: String? { get set }
```

## Discussion

Categories allow you to present custom actions to the user on your push notifications. For more information, see UIMutableUserNotificationCategory.

## See Also

### Grouping Notifications

var collapseIDKey: String?

A value that the system uses to coalesce unseen push notifications.

