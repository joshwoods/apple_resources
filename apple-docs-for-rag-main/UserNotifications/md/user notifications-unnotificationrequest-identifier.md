

- User Notifications
- UNNotificationRequest
-  identifier 

Instance Property

# identifier

The unique identifier for this notification request.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.14+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
var identifier: String { get }
```

## Discussion

Use this string to identify notifications in your app. For example, you can pass this string to the removePendingNotificationRequests(withIdentifiers:) method to cancel a previously scheduled notification.

If you use the same identifier when scheduling a new notification, the system removes the previously scheduled notification with that identifier and replaces it with the new one.

For local notifications, the system sets this property to the value passed to the request’s initializer (see the init(identifier:content:trigger:) method). For remote notifications, the system sets this property to the value of the `apns-collapse-id` key that you specified in the APNs request header when generating the remote notification. If your app doesn’t set a value, the system automatically assigns an identifier.

## See Also

### Getting the Request Details

var content: UNNotificationContent

The content associated with the notification.

var trigger: UNNotificationTrigger?

The conditions that trigger the delivery of the notification.

